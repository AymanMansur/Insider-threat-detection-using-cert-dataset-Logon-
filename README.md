# Insider-threat-detection-using-cert-dataset-Logon-

I used the CERT Insider Threat Detection Dataset, specifically the logon.csv file, to detect anomalies in user activity. To focus on a single user, I first filtered out their logon records.

Data Preprocessing
Defined working hours (6 AM - 6 PM) and non-working hours (6 PM - 6 AM).
Segmented logon activity based on these time frames.
Feature Extraction for Anomaly Detection
Daily Session Duration (Non-Working Hours):
The user logs on and off from multiple PCs daily.
Calculated session duration per PC and summed them to get the total session duration per day.
Daily Logon and Logoff Frequency (Non-Working Hours):
Counted the number of logons and logoffs during non-working hours.
Anomaly Detection
Applied Isolation Forest to identify unusual patterns in non-working hour activities.****
