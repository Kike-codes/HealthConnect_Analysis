# HealthConnect Clinic Appointment Attendance & No-Show Analysis

## Project Overview

This project analyzes appointment attendance and no-show patterns for HealthConnect Clinic using 5,000 appointment records.

The analysis focuses on understanding appointment outcomes and identifying factors associated with missed appointments. The project was developed using Excel, Power Query and Power BI, with supporting documentation created throughout the analysis process.

## Business Problem

HealthConnect Clinic needs to better understand appointment attendance and missed appointments in order to identify patterns that may support improved appointment management and patient engagement.

The analysis explores appointment outcomes, patient characteristics, previous appointment behaviour, booking lead time, reminder activity, distance to the clinic and waiting time.

## Dataset

- 5,000 appointment records
- 18 variables
- 1,696 unique patients
- Appointment outcomes: Attended, No-Show and Cancelled

The cleaned dataset is available in the `data` folder.

## Key KPIs

| KPI | Result |
|---|---:|
| Total Appointments | 5,000 |
| Attendance Rate | 48.8% |
| No-Show Rate | 51.2% |
| Cancellation Rate | 5.3% |
| Average Booking Lead Time | 29.6 days |

## Key Findings

### 1. Previous No-Show History

Patients with previous no-show records had higher current no-show rates.

- No previous no-shows: 46.3%
- 1 previous no-show: 55.9%
- 2+ previous no-shows: 63.5%

This suggests that previous appointment behaviour may be useful as an operational risk indicator.

### 2. Booking Lead Time

No-show rates increased as booking lead time increased.

- 0–3 days: 26.6%
- 4–7 days: 32.3%
- 8–14 days: 35.2%
- 15–30 days: 45.5%
- 31+ days: 63.9%

Appointments booked further in advance showed a substantially higher no-show rate.

### 3. Reminder Status

Appointments associated with a reminder had a higher attendance rate than appointments without a recorded reminder.

- Reminder sent: 50.1% attendance
- No reminder: 45.4% attendance

This represents an attendance difference of approximately 4.8 percentage points.

### 4. Distance to Clinic

Among appointments with recorded distance information, patients located 21+ km from the clinic had a higher no-show rate than those located 0–5 km away.

- 21+ km: 60.5%
- 0–5 km: 48.7%

This indicates that accessibility and travel distance may warrant further investigation.

### 5. Appointment Outcomes

No-shows represented 51.2% of non-cancelled appointments, highlighting a significant opportunity to improve appointment attendance.

## Recommendations

1. Introduce targeted follow-up for patients with previous no-show history.
2. Consider additional confirmation or reminder strategies for appointments booked far in advance.
3. Review reminder coverage and opportunities to improve patient engagement.
4. Investigate accessibility challenges affecting patients travelling longer distances.
5. Use previous attendance behaviour as an operational indicator when prioritising follow-up.

## Data Quality and Limitations

The dataset was reviewed for missing values, duplicates, inconsistent values and date-related issues.

Missing values for reminder channel, distance to clinic and waiting time were retained rather than artificially imputed.

Repeated patient IDs were retained because a patient may legitimately have multiple appointments.

No-show rate was calculated using Attended and No-Show appointments, while Cancelled appointments were treated separately.

The findings describe associations in the available data and should not be interpreted as evidence of causation.

## Cross-Track Collaboration

A simulated discussion with the Product/Business Analysis track focused on translating the appointment attendance findings into practical clinic operations. Key areas discussed included previous no-show behaviour, booking lead time, reminder coverage and patient distance. The input helped strengthen the recommendations by connecting the analytical findings to targeted patient follow-ups and improved appointment management.

## Tools Used

- Microsoft Excel
- Power Query
- Microsoft Power BI
- DAX
- GitHub

## Repository Structure

```text
HealthConnect_Analysis
│
├── data/
│   └── Healthconnect appointment data(cleaned).xlsx
│
├── documentation/
│   ├── Healthconnect initial data analysis.pdf
│   ├── Healthconnect Clinic Project summary.pdf
│   ├── HealthConnect Week 5 Analysis.pdf
│   └── HealthConnect Week 5 Project Summary.pdf
│
├── dashboard/
│   ├── HealthConnect Week 5 Dashboard.pdf
│   ├── HealthConnect Dashboard Overview.png
│   └── HealthConnect No-Show Drivers.png
│
├── HealthConnect Week 5 Dashboard.pbix
└── README.md
