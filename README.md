#  HealthConnect - Healthcare Appointment Analytics

> **Data Analytics Project | Patient Appointment Attendance & No-Show Analysis**

HealthConnect is a healthcare analytics project focused on understanding patient appointment attendance and no-show patterns and translating data findings into practical operational decision support.

The project progressed from data preparation and exploratory analysis to KPI development, advanced segmentation, Power BI dashboard development, testing, validation, and business recommendations.

---

##  Business Problem

Missed healthcare appointments can affect patient access, appointment availability, clinic capacity, and operational planning.

The goal of this project was to analyze appointment data to:

- Understand attendance, no-show, and cancellation patterns
- Identify patient and appointment characteristics associated with no-shows
- Develop meaningful appointment KPIs
- Explore patterns across different patient and appointment segments
- Build an interactive Power BI dashboard
- Validate analytical outputs through structured testing
- Translate findings into practical recommendations for appointment management

---

##  Dataset

The analysis used **5,000 healthcare appointment records** containing **18 variables**.

The dataset included information relating to:

- Patient characteristics
- Appointment type
- Appointment dates and booking lead time
- Previous no-show history
- Reminder status and channel
- Distance
- Waiting time
- Appointment outcome

### Appointment Outcomes

| Outcome | Records |
|---|---:|
| Attended | 2,314 |
| No-Show | 2,423 |
| Cancelled | 263 |
| **Total** | **5,000** |

Cancelled appointments were retained as a separate outcome.

---

##  Tools & Skills

**Tools**

- Microsoft Excel
- Power Query
- SQL
- Power BI
- DAX

**Skills Applied**

- Data cleaning and transformation
- Exploratory data analysis
- KPI development
- Data segmentation
- Data visualization
- Dashboard development
- Data validation
- Business insight generation
- Decision support

---

##  Analytical Workflow

```text
Raw Data
   ↓
Data Understanding
   ↓
Data Cleaning & Transformation
   ↓
KPI Development
   ↓
Exploratory Analysis
   ↓
Patient & Appointment Segmentation
   ↓
Advanced Analysis
   ↓
Power BI Dashboard
   ↓
Testing & Validation
   ↓
Business Insights
   ↓
Decision Support

⸻

Final Key Performance Indicators
 
KPI                          Result

Total Appointments           5,000

Attendance Rate              48.8%

No-Show Rate*                51.2%

Cancellation Rate             5.3%

Average Booking Lead Time     29.6 days
The no-show rate uses attended and no-show appointments as the denominator, with cancelled appointments treated separately.

⸻

 Key Findings

1. Previous No-Show History

No-show rates increased across previous no-show groups:


Previous No-Shows            No-Show Rate

0                              46.3%

1                              55.9%

2+                             63.5%

Patients with repeated previous no-shows represented an important segment for targeted appointment-management attention.

⸻

2. Booking Lead Time

Longer booking lead times were associated with higher no-show rates:
Booking Lead Time            No-Show Rate

0–3 days                      26.6%

4–7 days                      32.3%

8–14 days                     35.2%

15–30 days                    45.5%

31+ days                      64.0%

Appointments booked substantially in advance may therefore benefit from additional confirmation closer to the appointment date.

⸻

3. Reminder Patterns

Appointments associated with a recorded reminder had a higher attendance rate than those without a recorded reminder.
Reminder                  Attendance Rate

No reminder                  45.4%

Reminder sent                50.1%

This represents an attendance difference of approximately *4.8 percentage points*.

This finding represents an association in the observed data and does not establish that reminders caused the difference.

⸻

4. Distance

Longer travel distances were associated with higher no-show rates:
Distance                  No-Show Rate

0–5 km                        48.7%

5–10 km                       49.3%

11–20 km                      52.3%

21+ km                        60.5%

The 21+ km group showed a notably higher no-show rate, suggesting that access-related factors may warrant further investigation.

⸻

📊 Power BI Dashboard

The dashboard was developed as a three-page decision-support tool.

Page 1 — Appointment Overview

Provides a high-level view of:

* Total appointments
* Attendance rate
* No-show rate
* Cancellation rate
* Average booking lead time
* Appointment outcomes
* No-show patterns by time, day, appointment type, and age group

Page 2 — No-Show Drivers & Patient Behaviour

Explores:

* Previous no-show history
* Reminder status and channel
* Booking lead time
* Distance
* Waiting time
* Patient and appointment segments

Interactive slicers allow users to explore patterns across selected characteristics.

Page 3 — Advanced Analysis & Decision Support

Combines multiple characteristics to provide deeper insight, including:

* Previous No-Show History × Reminder Status
* Booking Lead Time × Reminder Status
* Previous No-Show History × Reminder Status — Attendance
* Distance × Appointment Type

⸻

 Testing & Validation

Testing was conducted to validate the reliability and usability of the analytical outputs.

The testing process included:

* KPI validation
* Analytical output validation
* Dashboard filter interaction testing
* Advanced analysis validation
* Missing-value handling
* Dashboard usability review
* End-to-end validation

A discrepancy was identified in two values within the Previous No-Show History × Reminder Status visual when compared with independent validation.

The discrepancy was investigated using Power BI’s Show as Table functionality and documented for further calculation/filter-context review rather than changing the dashboard without sufficient evidence.

⸻

 Business Insights

The analysis highlighted several areas that can support appointment-management decisions:

* Patients with repeated previous no-shows showed higher future no-show rates.
* Longer booking lead times were associated with substantially higher no-show rates.
* Appointments associated with reminders showed higher attendance.
* Longer travel distances were associated with higher no-show rates.
* Combining multiple patient and appointment characteristics provides more context than relying only on overall averages.

⸻

Recommendations

1. Target repeated no-show patients with appropriate appointment reminders and confirmation touchpoints.
2. Provide additional attention to long-lead appointments, particularly appointments booked 31+ days ahead.
3. Investigate access-related barriers for patients travelling longer distances, particularly those travelling 21+ km.
4. Use segmented analysis when designing appointment-management strategies rather than relying solely on overall no-show rates.
5. Monitor future interventions to evaluate whether attendance patterns change after implementation.

⸻

⚠️ Limitations

* The analysis identifies associations and does not establish causality.
* Some variables contained missing values, which were retained where appropriate.
* Waiting time was treated cautiously because it may contain information that would not be available before an appointment.
* Some segment-level comparisons may contain fewer observations than the overall dataset.
* A validation discrepancy remained documented for further review in the Previous No-Show × Reminder analysis.

⸻


##  Project Development

The HealthConnect project evolved through the following stages:

| Stage | Focus |
|---|---|
| **1. Problem Definition & Data Understanding** | Defined the healthcare attendance problem and reviewed the appointment dataset |
| **2. Data Preparation & KPI Development** | Cleaned and transformed the data and established core appointment KPIs |
| **3. Exploratory & Segmented Analysis** | Investigated attendance patterns across patient and appointment characteristics |
| **4. Advanced Analysis & Decision Support** | Examined relationships between key factors and developed actionable insights |
| **5. Dashboard Development** | Built an interactive Power BI dashboard for analysis and decision support |
| **6. Testing & Validation** | Validated KPIs, analytical outputs, dashboard interactions, and data handling |
| **7. Final Insights & Recommendations** | Translated validated findings into business insights and operational recommendations |

⸻

Final Outcome

HealthConnect demonstrates an end-to-end analytics workflow:

Data → Analysis → KPIs → Dashboard → Testing → Validation → Insights → Recommendations

The project shows how healthcare appointment data can be transformed into clear analytical findings and practical decision-support recommendations.

⸻

👩🏽‍💻 Author

Kikelomo Adesanya

Data Analyst | Excel | SQL | Power BI | Power Query


⸻

 Thank you for exploring HealthConnect!
