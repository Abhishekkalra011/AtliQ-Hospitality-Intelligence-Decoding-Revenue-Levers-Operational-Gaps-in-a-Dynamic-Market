# AtliQ-Hospitality-Intelligence-Decoding-Revenue-Levers-Operational-Gaps-in-a-Dynamic-Market
## interactive Webpage View

## Description Report view
https://app.powerbi.com/view?r=eyJrIjoiNjJhNWU5MTItODFkOC00NjFiLWJmYmQtOTI3MTY4N2Y2OWMxIiwidCI6IjU1YmQ5ZTdkLTdkMWEtNGZlNy1hNmZmLTJhOWY0YzdkZjAxYSJ9
![image](https://github.com/user-attachments/assets/cb05f896-af73-4ff7-8440-2fcdb5e49c37)

## Description
A data-driven exploration of AtliQ’s hospitality performance (May–July 2022), leveraging Power BI to uncover actionable insights on revenue optimization, booking trends, and customer satisfaction. Designed to empower stakeholders with strategies aligned with global hospitality benchmarks.
## Project Overview
### Business Problem
Post-pandemic, the hospitality industry faces volatile demand, rising cancellations, and shifting traveler preferences. AtliQ’s properties struggle with inconsistent occupancy (40.88% avg.), high cancellations (24.95%), and revenue leakage from underperforming room categories. The project identifies actionable levers to stabilize revenue, enhance guest loyalty, and align operations with modern traveler expectations.
### Objective
- Identify top revenue drivers (room classes, cities, platforms).
- Diagnose booking cancellation root causes.
- Benchmark property performance against industry standards.
vRecommend data-backed strategies for occupancy and rating improvements.
### Target Audience
#### C-Suite Executives: 
Strategic decision-making for portfolio optimization.
#### Revenue Managers: 
Dynamic pricing and OTA partnership strategies.
#### Operations Teams: 
Service quality improvements for low-rated properties.
#### Marketing Teams: 
Campaigns targeting high-value Elite customers.
## Data Structure & Data Model
![Hospitality analysis](https://github.com/user-attachments/assets/e7da9c41-7081-4f80-99fa-8ed5c54a91c4)

### Data Sources
#### dim_rooms: 
Room categories (RT1–RT4), classifications (Elite, Premium).
#### dim_hotels: 
Property details (Atliq Exotica, Palace, etc.), cities (Mumbai, Delhi).
#### dim_date: 
Temporal data (day types, month-year trends).
#### fact_aggregated_bookings: 
Capacity, successful bookings, occupancy rates.
#### fact_bookings: 
Granular booking data (platforms, cancellations, revenue).
### Data Cleaning
- Removed duplicates in booking IDs.Standardized city names (e.g., “B’lore” → “Bangalore”).

- Impute missing ratings using property-specific averages.

- Normalized revenue metrics to INR for consistency.
### Data Model
#### Star Schema: 
Central fact_bookings linked to dim_rooms, dim_hotels, and dim_date.
#### Key Relationships:
fact_bookings[room_class] → dim_rooms[room_category]
fact_bookings[property_name] → dim_hotels[property_id]
fact_bookings[check_in_date] → dim_date[date_key]
### Tools Used
#### Power BI: 
Interactive dashboards for real-time KPI tracking (revenue, cancellations, ratings).
#### Excel: 
Initial data profiling, outlier detection, and trend validation.
## Executive Summary
### Key Findings
#### Revenue Goldmine: 
RT2 rooms drive 32.8% of revenue, yet Mumbai’s Elite segment alone contributes 13.55% —untapped potential for premiumization.
#### Cancellation Crisis: 
May saw 45,882 cancellations (25.09% rate), costing ~₹99M. Direct offline bookings lagged OTAs by 298%.
#### Rating Paradox: 
Atliq Blu (3.96/5) outperforms, while Atliq Seasons (2.34/5) risks brand erosion.
#### Temporal Volatility: 
July’s revenue dropped 28.17% in its final week, mirroring post-holiday slumps in global markets.
### Impact
#### Revenue Boost: 
Optimizing RT2 pricing could yield ₹20M+ monthly.
#### Cancellation Reduction: 
Flexible policies may recover ₹30M annually.
#### Brand Equity:
Raising Atliq Seasons’ rating to 3.0+ could increase occupancy by 15%.
## Insights Deep-Dive
![image](https://github.com/user-attachments/assets/5d7358ad-58f8-4040-9a2c-847523a09cc4)

### Overall Performance
- Week 19’s 3.65 rating (+1.57% vs. Week 22) correlates with 44% occupancy—peak performance during pre-monsoon travel.

- Elite rooms generate ₹191M revenue (47.8M avg.), but Mumbai’s Elite segment contributes 13.55%—highlighting city-specific premium demand.

  ![image](https://github.com/user-attachments/assets/732f5773-f67e-4f5d-9ffb-7c602c73f2f0)

### Revenue Dynamics
- RT2’s ₹187.9M revenue (80.88% > RT1) aligns with global luxury traveler preferences.

- July 1 revenue spike (Mumbai: 39.23%) is tied to corporate events—the untapped opportunity for B2B partnerships.

  ![image](https://github.com/user-attachments/assets/801e2041-db14-4f0e-8c73-4f0b38241aad)

### Booking Trends
- Makeyourtrip dominates (26,898 bookings), but direct channels lag—a ₹28M revenue leak due to OTA commissions.

- May’s 45,882 cancellations (₹99M loss) were linked to rigid policies—compared to Marriott’s 18% cancellation rate post-flexibility rollout.

  ![image](https://github.com/user-attachments/assets/5389544c-7ee6-4d77-a169-7203a3a836a4)

### Ratings & Capacity
- Atliq Blu’s 3.96 rating reflects superior amenities, while Atliq Seasons’ 2.34 signals operational gaps (e.g., housekeeping delays).

- RT2’s 36.78% bookings vs. RT4’s 11.94% highlights misaligned inventory vs. demand.
## Recommendations
### Actionable Recommendations
#### Premiumization Strategy:
Launch “Elite Plus” packages for RT2 with personalized services (e.g., airport transfers).
#### Dynamic pricing: 
Adjust RT2 rates by ±15% during peak/off-peak days.
#### OTA Partnership Optimization:
Negotiate lower commissions with MakeYourTrip for bulk bookings.
Boost direct bookings via app-exclusive discounts (e.g., “Book Direct, Save 12%”).
#### Cancellation Mitigation:
Introduce tiered cancellation fees (e.g., 10% fee for cancellations <7 days prior).
#### Low-Rating Turnaround:
Deploy mystery shoppers at Atliq Seasons to identify service gaps.
### Business Impact
#### ₹50M+ Annual Revenue Gain: 
From RT2 optimization and OTA renegotiations.
#### 15% Occupancy Increase: 
At Atliq Seasons via service recovery initiatives.
#### 10% Commission Savings: 
By shifting 20% of bookings to direct channels.
## Skills Demonstrated
### Technical Skills
#### Advanced DAX: 
Calculated MTD revenue trends and cancellation rate cohorts.
#### Data Modeling: 
Star schema for efficient cross-dimensional analysis.
#### Predictive Analytics: 
Identified July’s revenue drop using time-series decomposition.
### Soft Skills
#### Stakeholder Communication: 
Translated RT2’s 32.8% revenue share into boardroom-ready strategies.
#### Problem-Solving: 
Addressed May’s cancellation spike with policy redesign.
## Challenges & Learnings
### Challenges
- Data inconsistencies in city naming (e.g., “Hyd” vs “Hyderabad”).
- Limited sustainability metrics (critical for modern ESG reporting).
### Learnings
- Temporal trends (e.g., weekend slumps) require hyper-localized campaigns.
- Direct booking incentives must balance short-term revenue vs. long-term brand loyalty.
