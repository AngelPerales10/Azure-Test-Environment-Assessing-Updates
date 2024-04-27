# Azure Test Environment to Assess Updates Within Microsoft Defender For Cloud

![Diagram](https://github.com/AngelPerales10/Azure-Test-Environment-Assessing-Updates/assets/108242721/ce9c0d47-cbd9-4c24-8bc7-8649056d4664)

## Introduction
Recently, changes were made to the settings of Microsoft Defender for Cloud within the subscription resource settings. These modifications primarily affected the environmental settings, particularly in the continuous export sections. These settings dictate how various data types are exported and transmitted to the Log Analytics Workspace. However, the alterations were implemented in a manner unfamiliar to users, including myself.

## Testing Environment Establishment

To address this issue, a testing environment was established to select and evaluate settings and configurations. The aim was to ensure that resources could still effectively transmit their security events and logs to the Log Analytics Workspace following the update. The testing environment consisted of the following components:

1. **Virtual Machines (1x Windows):** Used to simulate various system configurations and generate security events for testing purposes.

2. **Log Analytics Workspace with Kusto Query Language (KQL) Queries:** Employed for analyzing and querying the collected security event data.

3. **Microsoft Defender for Cloud:** Utilized to protect cloud resources and monitor security events.

4. **Azure Storage Account for Data Storage:** Enabled for storing the exported security event data before transmission to the Log Analytics Workspace.

5. **Windows Remote Desktop for Remote Access:** Facilitated remote access to the virtual machines for configuration and testing purposes.

## Testing Process

1. **Configuration Selection:** Different settings and configurations within Microsoft Defender for Cloud were evaluated to determine their impact on data export and transmission.

2. **Monitoring and Analysis:** The Log Analytics Workspace was continuously monitored, and KQL queries were employed to analyze the collected data for any discrepancies or issues.

3. **Validation:** The effectiveness of the selected settings was validated by ensuring that security events and logs were successfully transmitted to the Log Analytics Workspace without any loss or disruption.

## Final Results

![Pasted image 20240426172058](https://github.com/AngelPerales10/Azure-Test-Environment-Assessing-Updates/assets/108242721/5e1e8254-faab-4a5d-91e2-d7894296b1b9)

## Conclusion

Through testing and evaluation in the established environment, it was confirmed that the modified settings within Microsoft Defender for Cloud did not hinder the transmission of security events and logs to the Log Analytics Workspace. This process not only addressed the initial unfamiliarity with the changes but also ensured the continued effectiveness of security monitoring and response mechanisms within the cloud environment.
