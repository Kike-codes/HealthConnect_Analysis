# HealthConnect Appointment Attendance & No-Show Analysis

## Project Overview

HealthConnect is a healthcare appointment analytics project focused on understanding appointment attendance and no-show patterns and translating data-driven findings into decision support.

The project was developed as part of the AnalystLab Africa Experience Lab.

## Dataset

The analysis uses 5,000 appointment records containing patient, appointment, reminder, booking and attendance-related information.

The project examines:
- Appointment outcomes
- Attendance and no-show rates
- Previous no-show history
- Booking lead time
- Reminder status and channel
- Distance to clinic
- Appointment type
- Other relevant appointment characteristics

## Week 5 — Initial Analysis

Week 5 established the baseline analysis and a two-page Power BI dashboard covering appointment outcomes, attendance and no-show patterns.

Key baseline KPIs included:

- Total appointments: 5,000
- Attendance rate: 48.8%
- No-show rate: 51.2%
- Cancellation rate: 5.3%
- Average booking lead time: 29.6 days

## Week 6 — Advanced Analytics & Decision Support

Week 6 extended the Week 5 analysis through deeper segment-level investigation and KPI validation.

Four advanced analyses were developed:

1. Previous No-Show History × Reminder Status
2. Booking Lead Time × Reminder Status
3. Previous No-Show History × Reminder Status — Attendance
4. Distance × Appointment Type

### Key Findings

- Reminder-associated no-show rates were lower among patients with previous no-shows, with the largest difference among patients with 2+ previous no-shows.
- No-show rates increased as booking lead time increased, with the highest rates among appointments booked 31+ days ahead.
- The largest reminder-associated attendance difference occurred among patients with 2+ previous no-shows.
- No-show rates were generally highest for appointments 21+ km from the clinic.

## Decision Support

The Week 6 analysis highlighted three areas for further operational attention:

- Prioritising patients with repeated previous no-shows for targeted reminders and appointment confirmation.
- Considering additional confirmation touchpoints for appointments booked well in advance.
- Reviewing access and attendance support for patients travelling longer distances to the clinic.

These recommendations are based on observed associations and should be validated through further testing.

## KPI Definitions

Attendance and no-show rates use attended and no-show appointments as the denominator, with cancelled appointments treated separately.

## Limitations

The analysis is observational and does not establish causal relationships.

Missing values were retained rather than artificially imputed where appropriate. Waiting time was not treated as a primary predictive driver because it may contain post-appointment information.

## Cross-Track Integration

Week 6 analytical findings were shared with the Data Science track to support consideration of relevant variables and patterns for future predictive modelling.

Where further feedback was unavailable within the Week 6 timeframe, the Data Analytics deliverables were completed independently in accordance with project guidance.

## Repository Structure

- `data/` — project data and supporting data resources
- `analysis/` — analytical work
- `dashboard/` — Power BI dashboard files and screenshots
- `documentation/` — project reports and documentation
- `evidence/` — Week 6 supporting evidence

## Week 7 Focus

The next stage will focus on testing the identified patterns further, assessing modelling readiness, validating important variables and incorporating relevant cross-track feedback when available.
# HealthConnect Appointment Attendance & No-Show Analysis

## Project Overview

This project analyzes healthcare appointment attendance and no-show behaviour using the HealthConnect appointment dataset.

The analysis was developed as part of the AnalystLab Africa Experience Lab and progressed from exploratory analysis in Week 5 to advanced analysis in Week 6 and structured testing, refinement and validation in Week 7.

## Week 7: Testing, Refinement & Validation

Week 7 focused on validating the Week 6 Data Analytics outputs rather than rebuilding the analysis.

### Testing Activities

- KPI validation
- Advanced analytical output validation
- Dashboard cross-filter interaction testing
- Dashboard slicer testing
- Missing-value handling validation
- Dashboard usability review
- End-to-end analytical validation

### Key Validation Results

The main dashboard KPIs were validated successfully:

- Total Appointments: 5,000
- Attendance Rate: 48.8%
- No-Show Rate: 51.2%
- Cancellation Rate: 5.3%
- Average Booking Lead Time: 29.6 days

Most tested advanced analytical outputs were consistent with independently validated results.

A discrepancy was identified in two values within the Previous No-Show History × Reminder Status visual and was documented for further calculation/filter-context review.

## Key Insights

- Previous no-show history remains an important segmentation variable for attendance analysis.
- No-show rates increase across longer booking lead-time groups.
- Appointments associated with reminders showed different attendance patterns across patient segments.
- Appointments involving greater distance from the clinic showed relatively higher no-show rates in several segments.

These findings represent observed associations and should not be interpreted as causal effects.

## Data Quality & Limitations

- Missing values were retained rather than incorrectly imputed.
- Cancelled appointments were treated separately from attended and no-show appointments.
- The analysis is observational and does not establish causality.
- Waiting time was treated cautiously because it may contain post-appointment information.
- Cross-track testing was not completed during Week 7 because a collaborating track was unavailable.

## Tools

- Power BI
- Excel
- Power Query
- Microsoft Word
- GitHub

## Week 7 Evidence

Testing records and supporting evidence are included in the repository folders.
