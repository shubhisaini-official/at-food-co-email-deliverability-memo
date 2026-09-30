# at-food-co-email-deliverability-memo
Subscriber re-engagement &amp; email deliverability decision memo for AT Food Co. Features recency-based lifecycle segmentation, hard suppression rules, outcome metrics (CTCR, RPM, UCR), and a 60-day sunset cadence.
# 🐶 AT Food Co. — Subscriber Re-Engagement & Email Deliverability Decision Memo
> **Lifecycle Email Marketing: Recency-Based Segmentation, Domain Health Protection, and Outcome-Driven Retention Analytics**

[![Domain](https://img.shields.io/badge/Domain-Lifecycle%20Marketing%20%7C%20Email%20Ops-orange)](#)
[![Stack](https://img.shields.io/badge/Stack-ESP%20Automation%20%7C%20Klaviyo%20%7C%20Deliverability-blue)](#)
[![Methodology](https://img.shields.io/badge/Methodology-Respectful%20Communication-green)](#)

---

## 📌 Executive Summary & Retention Problem

* **The Challenge:** **AT Food Co.** currently runs dual email streams: a specialized "Puppy Nutrition Trial" stream and a "General Adult Fresh Care" stream. Leadership noticed that long-time subscribers who outgrew puppy care were still being bombarded with puppy emails, while older subscribers were churning due to inbox fatigue.
* **The Solution:** A recency-based lifecycle segmentation strategy that enforces hard spam suppression, transitions expired life-stage subscribers, and establishes respectful communication cadences.
* **Core Objective:** Protect ISP sender reputation (Gmail/Yahoo/Outlook), eliminate wasteful sends, and replace deceptive open rates with outcome-focused financial metrics (RPM, CTCR, UCR).

---

## 🏗️ Segmentation Matrix & Subscriber Activity Payload

    Subscriber ID | Days Since Last Purchase | Emails Opened (Last 10) | Current Promo Stream | Unsubscribed / Spam? | Recommended Strategy
    --------------|--------------------------|-------------------------|----------------------|----------------------|---------------------------------------------
    S01           | 12 days                  | 8 / 10                  | Puppy Nutrition      | No                   | Maintain Active High-Intent Cadence
    S02           | 210 days                 | 1 / 10                  | Puppy Nutrition      | No                   | Transition off Puppy -> Adult Home Stream
    S03           | 5 days                   | 9 / 10                  | General Adult Fresh  | No                   | Maintain VIP High-Frequency Stream
    S04           | 300 days                 | 0 / 10                  | Puppy Nutrition      | Yes                  | IMMEDIATE HARD SUPPRESSION
    S05           | 45 days                  | 6 / 10                  | General Adult Fresh  | No                   | Maintain Active Core Track
    S06           | 400 days                 | 2 / 10                  | Puppy Nutrition      | No                   | Transition off Puppy -> Low-Frequency Nurture
    S07           | 8 days                   | 10 / 10                 | General Adult Fresh  | No                   | Maintain VIP High-Frequency Stream
    S08           | 150 days                 | 3 / 10                  | General Adult Fresh  | No                   | Move to Paced 30-Day Re-Engagement Stream
    S09           | 20 days                  | 7 / 10                  | Puppy Nutrition      | No                   | Maintain Active High-Intent Cadence
    S10           | 500 days                 | 0 / 10                  | General Adult Fresh  | Yes                  | IMMEDIATE HARD SUPPRESSION

---

## 🛑 Action Plan & Immediate Stream Transitions

1. **Hard Suppression & Legal Compliance (S04, S10):**
   * *Action:* Added to Master Suppression List across all ESP systems immediately.
   * *Justification:* Opt-out or spam complaint flags must be respected 100% to protect domain sender authority.

2. **Life-Stage Stream Pivot (S02, S06):**
   * *Action:* Remove from "Puppy Nutrition" stream; transition to "General Adult Fresh Care".
   * *Justification:* 210 to 400 days since purchase indicates the dog is no longer a puppy. Continued puppy emails irritate subscribers and drive spam flags.

3. **VIP Active Stream Maintenance (S01, S03, S05, S07, S09):**
   * *Action:* Maintain regular weekly delivery.
   * *Justification:* Recent purchases (<45 days) and high open engagement demonstrate active customer value.

4. **At-Risk Paced Re-Engagement (S08):**
   * *Action:* Shift from weekly blasts to a 21–30 day low-frequency nurture stream.
   * *Justification:* 150 days without purchase signals early churn risk. Over-messaging will trigger unsubscribes[cite: 1, 2].

---

## 📈 Outcome-Driven Metrics vs. Vanity Open Rates

Apple Mail Privacy Protection (MPP) auto-loads tracking pixels, making raw Open Rates artificial and misleading[cite: 1, 2]. We measure email success using 4 commercial health metrics[cite: 1, 2]:

    Metric Name                     | Formula / Definition                                      | Strategic Objective
    --------------------------------|-----------------------------------------------------------|--------------------------------------------------
    Click-to-Conversion Rate (CTCR) | (Completed Orders / Unique Clicks) * 100                 | Evaluates landing page relevance & buying intent
    Revenue Per Mille (RPM)         | (Net Revenue / Total Emails Delivered) * 1,000            | Measures financial dollar yield per 1,000 sends
    Unsubscribe-to-Click Ratio (UCR)| (Total Unsubscribes / Unique Clicks) * 100                | Measures email friction (>20% signals bad content)
    Inbox Placement Rate            | % of emails landing in Inbox vs Spam (Target: >99%)       | Measures domain health & ISP trust (Gmail/Yahoo)

---

## ⏳ 60-Day Sunset & Re-Engagement Cadence

For moderate-recency candidates (S08, S02, S06)[cite: 1, 2]:

* **Day 0:** Send low-pressure preference check (*"Would you like fewer emails or different recommendations?"*)[cite: 1, 2].
* **Day 21:** Send non-promotional, high-utility care guide (*"3 Signs Your Dog's Digestion Needs Fresh Greens"*)[cite: 1, 2].
* **Day 45:** Send soft trial re-engagement offer with zero expiration pressure[cite: 1, 2].
* **Day 60 (Sunset Clause):** If zero clicks occur after 60 days, move subscriber to a quarterly digest to safeguard deliverability[cite: 1, 2].
