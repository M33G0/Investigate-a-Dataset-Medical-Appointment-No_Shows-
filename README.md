# Investigate a Dataset: Medical Appointment No Shows

## Project Overview
This project performs an exploratory data analysis (EDA) on a dataset containing 100k medical appointments from the public health system in Brazil. The primary objective is to analyze the factors associated with whether patients show up for their scheduled appointments or miss them ("No-Show"). 

## Dataset Structure
The dataset contains columns regarding patient demographics and medical conditions:
* **PatientId / AppointmentID:** Unique identifiers.
* **Gender & Age:** Patient demographics.
* **ScheduledDay / AppointmentDay:** Dates tracking when the appointment was registered vs. the actual visit date.
* **Neighbourhood:** Location of the hospital/clinic.
* **Scholarship:** Indicates whether or not the patient is enrolled in the Brazilian welfare program (Bolsa Família).
* **Hipertension, Diabetes, Alcoholism, Handcap:** Medical profile flags.
* **SMS_received:** Whether one or more reminder text messages were sent to the patient.
* **No-show:** 'No' if the patient showed up, and 'Yes' if they did not show up.

## Key Findings & Insights
* **Demographics:** Children and young families (ages 0-10) show higher attendance rates, indicating high parental care. 
* **Location:** The neighbourhood 'JARDIM CAMBURI' had the highest frequency of successful visits, suggesting optimized routes or better facility outreach.
* **SMS Reminders:** Counterintuitively, the preliminary analysis indicated that a large portion of patients who received an SMS still missed appointments, highlighting a potential area for strategy adjustments or further temporal analysis (e.g., timing of the SMS text).

## Limitations Note
The insights could be significantly enhanced if the dataset included details such as whether the appointment was an emergency, the specific clinical department scheduled, whether it was the patient's first time visiting, and the patient's subjective satisfaction score of past visits.

## Tech Stack
* Jupyter Notebook
* Python 3
* Pandas, NumPy, Matplotlib, Seaborn
