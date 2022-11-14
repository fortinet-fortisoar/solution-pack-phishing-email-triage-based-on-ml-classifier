# What's New

## Bugfixes

- Removed the **Scenario** module and its **System View Template (SVT)** from the solution pack since it is already a part of the SOC Simulator solution pack.
- The example alert generating playbook **Generate Phishing Email Alert** now creates alerts of type **Suspicious Email**.
- The response playbook **Phishing Email Triage Based On ML Classifier** is a manually-run playbook that now becomes available for execution for alerts of type **Suspicious Email**. Earlier it became available for alerts of type **Phishing**.
- A unique scenario **Phishing Email Triage Based On ML Classifier** is now created with the installation of this solution pack.