# SoteLogGuardian AI - Building AI course project

An AI-powered anomaly detection system designed to analyze patient information system logs, identifying unauthorized access and protecting patient privacy in healthcare and social care organizations.
The idea is part of the Building AI course project.

<img width="300" height="300" alt="aidatasecurity" src="https://github.com/user-attachments/assets/1b3d66d2-bf6f-46a1-8b83-4da3c30833b9" />

## 📋 Summary

Healthcare and social welfare organizations are legally mandated to monitor system logs to ensure data privacy. However, patient information systems generate thousands of log rows every single second. Human auditors cannot process this massive volume of data, leaving organizations reliant on inefficient random sampling. As a result, illegal "curiosity lookups" (e.g., healthcare staff accessing records of individuals without an active care relationship) frequently go unnoticed.
The idea is part of the Building AI course project.

**SoteLogGuardian AI** solves this by utilizing unsupervised machine learning to analyze the massive stream of log data in real-time. It automatically detects anomalous access patterns and flags high-risk incidents for Data Protection Officers (DPOs) to investigate.

The idea is part of the Building AI course project.

<img width="321" height="491" alt="logevents" src="https://github.com/user-attachments/assets/9df5b192-1ab0-445f-a4e9-3eb334e58932" />

---

## 🔍 Background

### The Problem
Patient records contain highly sensitive and confidential data. While legislation strictly forbids accessing records without a direct therapeutic or care relationship, current healthcare systems cannot natively prevent these actions at the user interface level. Security relies heavily on post-event log audits. Because the volume of data is humanly impossible to review, the probability of catching an insider threat or an unauthorized viewer is extremely low.

### Frequency & Impact
This is a widespread and highly publicized issue. News reports frequently expose instances where nurses, doctors, or administrative staff have illegally accessed the data of public figures, neighbors, or acquaintances. This undermines public trust in digital healthcare systems and creates heavy administrative and legal burdens for social and healthcare (Sote) organizations when breaches are eventually exposed.

### Personal Motivation
The primary motivation behind this project is to protect patient privacy and safeguard fundamental digital rights. By automating a critical compliance requirement, this solution alleviates the immense manual audit workload currently exhausting healthcare security teams, while drastically increasing the detection rate of unethical behavior.

---

## 🛠️ Data and AI Techniques

### AI Techniques
* **Anomaly Detection (Unsupervised Learning):** Since malicious lookups are rare compared to legitimate daily operations, algorithms like **Isolation Forest** or **Autoencoders** are trained on historical logs to map "normal" clinical workflows. Any transaction that deviates significantly (e.g., viewing a profile outside shift hours, or a sudden spike in lookups of unrelated individuals) is flagged.
* **Classification (Supervised Learning):** Once an organization accumulates historically verified breach data, classification models can be trained to recognize the specific behavioral signatures of "curiosity snooping."
* **Graph Neural Networks (GNNs):** Used to identify hidden relationships and networks between employees and patients (e.g., identifying if an employee is looking up individuals living in their own neighborhood or sharing social circles).

---

## 👥 How It Is Used

### Context & Implementation
LogGuardian AI is designed to run asynchronously on a dedicated log server—**it does not directly integrate into or modify the core patient information system's user interface.** This ensures that deployment does not cause downtime or interrupt critical medical software.

### Stakeholders & Viewpoints
* **Data Protection Officers (DPOs):** The direct users of the tool. They receive a clean dashboard highlighting aggregated risk scores and a pre-filtered list of the most critical anomalies, allowing them to initiate official investigations or police reports swiftly.
* **Healthcare Professionals:** Honest workers are protected from arbitrary random audits, while the presence of the system acts as a strong psychological deterrent for potential wrongdoers.
* **Patients:** Benefit from the assurance that their sensitive personal data is actively and comprehensively protected by modern technology.

---

## 🛠️ Data Sources and AI methods
The system operates as an independent backend analysis tool that ingests data from two primary sources:
1. **System Log Stream:** Continuous transactional logs containing `Timestamp`, `User ID`, `Professional Role`, `Patient ID`, and `Action Executed`. Shift schedules, active appointment registries, and department mapping to verify whether a professional has a legitimate reason to be interacting with a specific patient's file at that given time.

---

## ⚠️ Challenges

* **Reactive, Not Proactive:** Because this tool does not plug into the frontend of the patient information system, it cannot block a user from opening a file in real-time. It detects the violation minutes or hours after it occurs.
* **False Positives:** Medical emergencies (e.g., a critical patient rushed into the ER) require immediate data access without prior appointments or established care relationships. The AI will likely flag this as an anomaly. Therefore, **human verification is always mandatory** before any disciplinary or legal action is taken.

---

## 🚀 What's Next?

1. **Proactive Warnings:** As the AI model matures and achieves high accuracy, it could eventually be integrated directly into the patient information system interface. Instead of blocking access, it could trigger a real-time warning prompt when a high-risk lookup is attempted: *"Warning: No active care relationship detected. Please input your mandatory justification for viewing these records."*
2. **Cross-Sector Scaling:** The core anomaly detection framework developed here can easily be cross-trained to protect sensitive logs in other highly regulated sectors, such as law enforcement, tax administration, and banking.

---

## 📜 Acknowledgments

* **Inspiration:** This project is inspired by ongoing public discussions surrounding digital ethics, European GDPR enforcement, and the operational compliance challenges faced by the Nordic healthcare sector.
* **Open Source Technologies:** Built using open-source data streaming and machine learning frameworks including **Apache Kafka** for high-throughput log ingestion and **Scikit-Learn / PyTorch** for anomaly detection modeling.
# my-new-project
Building AI course project
