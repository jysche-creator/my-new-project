# SoteLogGuardian AI - Building AI course project

An AI-powered anomaly detection system designed to analyze patient information system logs, identifying unauthorized access and protecting patient privacy in healthcare and social care organizations.
The idea is part of the Building AI course project.

<img width="300" height="300" alt="aidatasecurity" src="https://github.com/user-attachments/assets/1b3d66d2-bf6f-46a1-8b83-4da3c30833b9" />

## 📋 Summary

Healthcare and social welfare organizations are legally mandated to monitor system logs to ensure data privacy. However, patient information systems generate thousands of log rows every single second. Human auditors cannot process this massive volume of data, leaving organizations reliant on inefficient random sampling. As a result, illegal "curiosity lookups" (e.g., healthcare staff accessing records of individuals without an active care relationship) frequently go unnoticed.
The idea is part of the Building AI course project.

**SoteLogGuardian AI** solves this by utilizing unsupervised machine learning to analyze the massive stream of log data in real-time. It automatically detects anomalous access patterns and flags high-risk incidents for Data Protection Officers (DPOs) to investigate.

The idea is part of the Building AI course project.

%3CmxGraphModel%3E%3Croot%3E%3CmxCell%20id%3D%220%22%2F%3E%3CmxCell%20id%3D%221%22%20parent%3D%220%22%2F%3E%3CmxCell%20id%3D%222%22%20edge%3D%221%22%20parent%3D%221%22%20source%3D%227%22%20style%3D%22edgeStyle%3DorthogonalEdgeStyle%3Brounded%3D0%3BorthogonalLoop%3D1%3BjettySize%3Dauto%3Bhtml%3D1%3BentryX%3D0%3BentryY%3D0.5%3BentryDx%3D0%3BentryDy%3D0%3BexitX%3D0.5%3BexitY%3D1%3BexitDx%3D0%3BexitDy%3D0%3B%22%20target%3D%228%22%3E%3CmxGeometry%20relative%3D%221%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%223%22%20edge%3D%221%22%20parent%3D%221%22%20source%3D%227%22%20style%3D%22edgeStyle%3DorthogonalEdgeStyle%3Brounded%3D0%3BorthogonalLoop%3D1%3BjettySize%3Dauto%3Bhtml%3D1%3BentryX%3D0%3BentryY%3D0.5%3BentryDx%3D0%3BentryDy%3D0%3BexitX%3D0.5%3BexitY%3D1%3BexitDx%3D0%3BexitDy%3D0%3B%22%20target%3D%229%22%3E%3CmxGeometry%20relative%3D%221%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%224%22%20edge%3D%221%22%20parent%3D%221%22%20source%3D%227%22%20style%3D%22edgeStyle%3DorthogonalEdgeStyle%3Brounded%3D0%3BorthogonalLoop%3D1%3BjettySize%3Dauto%3Bhtml%3D1%3BentryX%3D0%3BentryY%3D0.5%3BentryDx%3D0%3BentryDy%3D0%3BexitX%3D0.5%3BexitY%3D1%3BexitDx%3D0%3BexitDy%3D0%3B%22%20target%3D%2210%22%3E%3CmxGeometry%20relative%3D%221%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%225%22%20edge%3D%221%22%20parent%3D%221%22%20source%3D%227%22%20style%3D%22edgeStyle%3DorthogonalEdgeStyle%3Brounded%3D0%3BorthogonalLoop%3D1%3BjettySize%3Dauto%3Bhtml%3D1%3BentryX%3D0%3BentryY%3D0.5%3BentryDx%3D0%3BentryDy%3D0%3BexitX%3D0.5%3BexitY%3D1%3BexitDx%3D0%3BexitDy%3D0%3B%22%20target%3D%2211%22%3E%3CmxGeometry%20relative%3D%221%22%20as%3D%22geometry%22%3E%3CmxPoint%20x%3D%22415%22%20y%3D%22330%22%20as%3D%22sourcePoint%22%2F%3E%3C%2FmxGeometry%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%226%22%20edge%3D%221%22%20parent%3D%221%22%20source%3D%227%22%20style%3D%22edgeStyle%3DorthogonalEdgeStyle%3Brounded%3D0%3BorthogonalLoop%3D1%3BjettySize%3Dauto%3Bhtml%3D1%3BentryX%3D0.5%3BentryY%3D0%3BentryDx%3D0%3BentryDy%3D0%3B%22%20target%3D%2212%22%3E%3CmxGeometry%20relative%3D%221%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%227%22%20parent%3D%221%22%20style%3D%22rounded%3D1%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3B%22%20value%3D%22Log%20Event%20Data%26lt%3Bdiv%26gt%3B-%26amp%3Bnbsp%3BEvent%20ID%20%26amp%3Bamp%3B%20Technical%20details%26lt%3B%2Fdiv%26gt%3B%26lt%3Bdiv%26gt%3B-%26amp%3Bnbsp%3BUser%20Action%26lt%3B%2Fdiv%26gt%3B%22%20vertex%3D%221%22%3E%3CmxGeometry%20height%3D%2260%22%20width%3D%22170%22%20x%3D%22330%22%20y%3D%22260%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%228%22%20parent%3D%221%22%20style%3D%22rounded%3D1%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3B%22%20value%3D%22Data%20Processor%20Credentials%22%20vertex%3D%221%22%3E%3CmxGeometry%20height%3D%2260%22%20width%3D%22120%22%20x%3D%22530%22%20y%3D%22320%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%229%22%20parent%3D%221%22%20style%3D%22rounded%3D1%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3B%22%20value%3D%22Accessing%20System%20Data%22%20vertex%3D%221%22%3E%3CmxGeometry%20height%3D%2260%22%20width%3D%22120%22%20x%3D%22530%22%20y%3D%22390%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2210%22%20parent%3D%221%22%20style%3D%22rounded%3D1%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3B%22%20value%3D%22Customer%20information%22%20vertex%3D%221%22%3E%3CmxGeometry%20height%3D%2260%22%20width%3D%22120%22%20x%3D%22530%22%20y%3D%22460%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2211%22%20parent%3D%221%22%20style%3D%22rounded%3D1%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3B%22%20value%3D%22Access%20Context%20Metadata%26lt%3Bdiv%26gt%3B-%20Registry%20holder%26lt%3B%2Fdiv%26gt%3B%26lt%3Bdiv%26gt%3B-%26amp%3Bnbsp%3BPurpose%20of%20Use%26lt%3B%2Fdiv%26gt%3B%26lt%3Bdiv%26gt%3B-%20Method%20of%20use%26lt%3B%2Fdiv%26gt%3B%22%20vertex%3D%221%22%3E%3CmxGeometry%20height%3D%2280%22%20width%3D%22120%22%20x%3D%22530%22%20y%3D%22530%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3CmxCell%20id%3D%2212%22%20parent%3D%221%22%20style%3D%22rounded%3D1%3BwhiteSpace%3Dwrap%3Bhtml%3D1%3B%22%20value%3D%22Accessed%20Data%20Component%22%20vertex%3D%221%22%3E%3CmxGeometry%20height%3D%2260%22%20width%3D%22120%22%20x%3D%22355%22%20y%3D%22640%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3C%2Froot%3E%3C%2FmxGraphModel%3E

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
