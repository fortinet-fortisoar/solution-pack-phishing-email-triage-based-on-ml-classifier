| [Home](https://github.com/fortinet-fortisoar/solution-pack-phishing-email-triage-based-on-ml-classifier/blob/release/1.0.0/README.md) |
|--------------------------------------------|

# Usage

Refer to [Simulate Scenario documentation](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/docs/usage.md) to understand how to simulate and reset scenarios.

To understand the process FortiSOAR follows to triage the phishing emails based on ML classifier, we have included a scenario &mdash; **Phishing Email** with this solution pack. Refer to the section *Phishing Email Scenario* to understand how this solution pack's automation addresses your needs.

## Phishing Email Scenario
This scenario generates an example alert of Type *Suspicious Email* in FortiSOAR's **Alerts** module.

Navigate to the demo alert and note the following:

- The demo alert created is an example of a default email ingestion using the **Data Ingestion** feature
- Alert fields are mapped with information from the email, such as sender email id, reporter email id, and attachments
- Users can execute investigation playbook, out-of-the-box (OOB), against the alert **Phishing Email Triage Based On ML Classifier**. It utilizes email information (sender, receiver, subject, body, header, and sender domain) for analyzing the case and suggesting corrective action.

**Phishing Email Triage Based On ML Classifier**: Users can launch **Phishing Email Triage Based On ML Classifier** playbook from an alert. This playbook performs following automated tasks:

- Set the threshold value for confidence. Threshold identifies the confidence level above which we are sure that the email is phishing. 
- Provide verdict for the phising alert record to the FortiSOAR Phishing Classifier connector, which will return the "confidence", "status" and "label" as a response.
- Based on the response parameters and threshold value the triage action will perform.