<!-- This is the markdown template for the final project of the Building AI course, 
created by Reaktor Innovations and University of Helsinki. 
Copy the template, paste it to your GitHub README and edit! -->

# LogGuardian AI

Final project for the Building AI course

<img width="300" height="300" alt="aidatasecurity" src="https://github.com/user-attachments/assets/1b3d66d2-bf6f-46a1-8b83-4da3c30833b9" />

## Summary

LogGuardian AI is an automated anomaly detection system designed to monitor massive streams of healthcare log data in real-time. By utilizing machine learning, it identifies unauthorized record access and "curiosity snooping" by internal staff without an active care relationship. The system flags high-risk incidents automatically, protecting sensitive patient privacy while fulfilling legal auditing mandates efficiently.

<img width="321" height="491" alt="logevents" src="https://github.com/user-attachments/assets/9df5b192-1ab0-445f-a4e9-3eb334e58932" />


## Background

Social and healthcare organizations are legally mandated to monitor system logs to ensure data privacy, but patient information systems generate thousands of rows of data every single second.
* **Humanly Impossible Workload:** The sheer volume of log data makes manual auditing ineffective, forcing organizations to rely on random sampling.
* **Low Detection Rate:** Due to limited human resources, insider threats and unauthorized "curiosity lookups" (e.g., viewing records of neighbors or celebrities) rarely get caught.
* **Sensitive Data Exposure:** Patient records contain highly sensitive details, and unmonitored access severely undermines public trust in digital healthcare.


## How is it used?

LogGuardian AI operates as an independent backend analysis service running on log servers, meaning it does not directly modify or slow down the live patient information system. The direct users are Data Protection Officers (DPOs) who receive filtered, high-priority alerts on a dedicated security dashboard whenever an anomaly is detected.


## Data sources and AI methods

The project depends on integrating real-time system logs with internal metadata catalogs to contextually evaluate each transaction.

| Data Source | Description |
| ----------- | ----------- |
| **System Log Stream** | Continuous transactional rows containing Timestamp, User ID, Patient ID, and Action. |
| **Contextual Metadata** | HR work schedules, hospital department mappings, and active patient appointment lists. |

### AI Techniques:
* **Unsupervised Anomaly Detection:** Algorithms like *Isolation Forests* or *Autoencoders* are trained on historical logs to learn normal clinical workflows and isolate unique, non-standard access behaviors.
* **Supervised Classification:** Pattern recognition models trained on known, historically verified breach cases to identify the specific behavioral "fingerprint" of curiosity snooping.


## Challenges

* **Reactive Nature:** Because this solution is not integrated directly into the frontend user interface, it cannot block a user from opening a file in real-time. It detects the violation minutes or hours after it occurs.
* **False Positives:** Critical medical emergencies (e.g., a patient rushed into the ER) require immediate data access without prior appointments. The AI will flag these as anomalies, meaning **human-in-the-loop verification** by a DPO is always mandatory before taking legal action.
* **Ethical Considerations:** The system must strictly handle employee tracking data in compliance with labor privacy laws, ensuring it is used purely for data protection auditing rather than general performance monitoring.


## What next?

The project could scale from a post-event analysis tool into a proactive prevention platform by developing real-time frontend APIs. Instead of blocking access during a suspected anomaly, it could trigger a real-time justification prompt directly within the patient software interface. Furthermore, the core anomaly detection matrix could be cross-trained to safeguard sensitive logs in other strictly regulated sectors, such as law enforcement, tax administration, and banking.


## Acknowledgments

* **Inspiration:** Inspired by public discussions surrounding European GDPR compliance challenges, patient privacy rights, and logging guidelines provided by the Finnish National Architecture for Digital Services.
* **Open Source Technologies:** Built using conceptual frameworks from open-source machine learning libraries like Scikit-Learn and data streaming architectures like Apache Kafka.
