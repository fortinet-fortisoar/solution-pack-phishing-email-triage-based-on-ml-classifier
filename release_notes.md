# Fix Details

- Removed the `Scenario` module and its System View Template (SVT) from the solution pack since it's already a part of the SOC Simulator solution pack.
- The demo alert generation playbook `Generate Phishing Email Alert` will now create alerts of type `Suspicious Email`.
- The response playbook `Phishing Email Triage Based On ML Classifier` will now execute on alerts of type `Suspicious Email`.
- Now, A unique scenario `Phishing Email Triage Based On ML Classifier` will be created for the solution pack.