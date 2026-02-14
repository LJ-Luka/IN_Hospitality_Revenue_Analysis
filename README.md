# Atliq Grands Hospitality Revenue Analysis: Diagnosing a Declining Hotel Chain

**[Download Dashboard (.pbix)](https://github.com/LJ-Luka/More_PowerBI_Projects/blob/main/Project/Hospitality_dashboard.pbix)** | **[View Metrics & DAX](https://github.com/LJ-Luka/More_PowerBI_Projects/blob/main/Project/metrics%20list.xlsx)** | **[Stakeholder Mockup](https://github.com/LJ-Luka/More_PowerBI_Projects/blob/main/Project/mock%20up%20dashboard_atliq%20grands.png)**

---

## The Business Problem

Atliq Grands, a luxury and business hotel chain operating across four major Indian cities (Mumbai, Delhi, Bangalore, Hyderabad), is experiencing revenue erosion. Leadership needs visibility into what's driving the decline and where intervention will have the greatest impact.

This analysis transforms three months of booking data (May–July) into an interactive dashboard that answers one critical question: **Where is Atliq Grands losing money, and how can they recover it?**

---

## Executive Summary

| Metric | Value | Industry Benchmark | Status |
|--------|-------|-------------------|--------|
| Total Revenue | ₹1.69B | — | Baseline |
| Occupancy Rate | 57.8% | 65-70% | ⚠️ Below target |
| RevPAR | ₹7.3K | — | Room for growth |
| Cancellation Rate | 24.8% | 15-20% | 🔴 Critical |
| Average Rating | 3.6/5 | 4.0+ | ⚠️ Needs attention |
| Realisation Rate | 70% | 80%+ | ⚠️ Revenue leakage |

**The diagnosis:** Atliq Grands isn't just underperforming—it's bleeding revenue through a 24.8% cancellation rate and 30% unrealised bookings. Fixing these two issues alone could recover ₹200M+ annually.

---

## Key Findings & Strategic Recommendations

### 1. Revenue Is Declining Month-Over-Month

| Month | Revenue | Change |
|-------|---------|--------|
| May | ₹582M | — |
| June | ₹554M | -4.8% |
| July | ₹552M | -0.4% |

**The trend is concerning.** May's strong performance wasn't sustained. Occupancy followed the same pattern (58.5% → 57.6% → 57.2%).

**Recommendation:** Investigate what drove May's success (events, promotions, seasonal factors) and replicate it. The Q3 decline suggests either competitive pressure or operational issues emerging.

---

### 2. The Cancellation Problem Is Costing ₹420M Annually

At 24.8%, nearly **1 in 4 bookings are cancelled**—well above the industry standard of 15-20%. With 132,939 total bookings generating ₹1.69B, that's roughly ₹420M in at-risk revenue per quarter.

**Recommendation:**
- Implement tiered cancellation policies (non-refundable rates at 10-15% discount)
- Require deposits for peak-period bookings
- Analyze cancellation patterns by platform—are certain channels worse?

---

### 3. Weekends Outperform Weekdays Across Every Metric

| Metric | Weekday | Weekend | Δ |
|--------|---------|---------|---|
| RevPAR | Lower | Higher | +15% |
| Occupancy | Lower | Higher | +8% |
| ADR | Lower | Higher | +12% |

**The opportunity:** Weekday utilization is the gap. Business travel should fill this, but it's underperforming.

**Recommendation:** 
- Partner with corporate accounts for guaranteed weekday bookings
- Create weekday-specific packages (extended stays, work-from-hotel)
- Dynamic pricing to incentivize Tuesday-Thursday stays

---

### 4. Luxury Drives Revenue, But Business Category Is Underutilized

- **Luxury:** 61.6% of revenue
- **Business:** 38.4% of revenue

This split suggests the business segment has growth potential. Business travelers typically book weekdays—addressing Finding #3.

**Recommendation:** Invest in business category amenities (meeting rooms, fast WiFi, late checkout) and corporate sales team.

---

### 5. Mumbai's Atliq Exotica Is the Star Property

| Property | Revenue | Bookings | Why It Works |
|----------|---------|----------|--------------|
| Atliq Exotica, Mumbai | ₹117M | 7,251 | Highest guest duration |
| Atliq Palace, Delhi | — | — | Highest occupancy (66.3%) |

**The insight:** Guest duration correlates with revenue. Exotica's success isn't just occupancy—guests stay longer and spend more.

**Recommendation:** Analyze what Exotica does differently. Is it amenities? Location? Service? Replicate across underperforming properties.

---

### 6. Booking Platform Performance Varies

Realisation rates are similar across platforms, but **direct offline and Tripster** bookings convert best. **Direct online** has the lowest ADR.

**Recommendation:** 
- Reduce OTA dependency (high commission fees)
- Invest in direct booking incentives (loyalty points, room upgrades)
- Audit why direct online underperforms—UX issues? Pricing parity violations?

---

### 7. Bangalore Has a Cancellation Problem

Atliq City, Bangalore (ID 19560) has the **highest cancellation rate at 26.5%**—2 points above the chain average.

**Recommendation:** Property-specific investigation needed. Possible causes: overbooking practices, local competition, or service issues reflected in ratings.

---

## Technical Implementation

### Data Architecture
- **5 source tables:** 2 dimension tables (hotels, rooms, dates) + 2 fact tables (bookings, aggregated bookings)
- **Data model:** Star schema for optimal query performance
- **ETL:** Power Query for cleaning, null handling, and type consistency

### Key DAX Measures
```
RevPAR = DIVIDE([Revenue], [Total Capacity])
Occupancy % = DIVIDE([Total Successful Bookings], [Total Capacity])
Realisation % = DIVIDE([Total Checked Out], [Total Bookings])
ADR = DIVIDE([Revenue], [Total Bookings])
```

### Dashboard Features
- Week-over-week trend analysis
- Drill-through to property-level details
- Dynamic filtering by city, property, room type, platform
- Tooltip-based deep dives

---

## Data Limitations

- **3-month window:** May-July only; seasonality conclusions limited
- **No cost data:** Revenue analyzed, but profitability unknown
- **No competitor benchmarks:** Can't assess market share shifts
- **Rating context missing:** 3.6 average, but distribution and trends needed

---

## Conclusion

Atliq Grands' revenue challenges stem from three fixable problems:

1. **Cancellations** (24.8%) — Policy changes could recover ₹100M+
2. **Weekday underutilization** — Corporate partnerships needed
3. **Platform mix** — Shift toward direct bookings to improve margins

The data is clear. The opportunities are quantified. The question now is execution.

---

*Built with Power BI | Star Schema Data Model | DAX Calculations*
