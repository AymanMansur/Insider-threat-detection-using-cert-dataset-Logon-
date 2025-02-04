# **Anomaly Detection in Insider Threats using Logon Data**
## **Overview**
This project utilizes the **CERT Insider Threat Detection Dataset** (logon.csv) to identify anomalies in user activity, focusing on non-working hour behavior. By applying Isolation Forest, we detect potential insider threats based on deviations from normal usage patterns.

## **Methodology**
1. **Data Preprocessing**
Filtered logon records for a single user.
Defined working hours (6 AM - 6 PM) and non-working hours (6 PM - 6 AM).
Segmented logon data accordingly.
2. **Feature Engineering**
Daily Session Duration (Non-Working Hours):
The user logs on and off from multiple PCs daily.
Calculated session duration per PC and summed them for total session duration per day.
Daily Logon and Logoff Frequency (Non-Working Hours):
Counted the number of logons and logoffs during non-working hours.
3. **Anomaly Detection**
Applied Isolation Forest to detect anomalies in user behavior outside working hours.
Identified abnormal logon patterns that may indicate suspicious activity.
The approach can be extended to monitor multiple users for insider threat detection.
## **Technologies Used**
Python
Pandas (Data Processing)
Scikit-Learn (Machine Learning - Isolation Forest)
## Future Improvements
Expand analysis to multiple users.
Incorporate additional features like IP addresses and geolocation.
Test other anomaly detection techniques (e.g., One-Class SVM, Autoencoders).
Dataset Link: https://www.kaggle.com/datasets/mrajaxnp/cert-insider-threat-detection-research/data?select=logon.csv 
