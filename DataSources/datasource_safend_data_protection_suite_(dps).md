Vendor: Safend
==============
Product: Data Protection Suite (DPS)
------------------------------------
|                              Use-Case                               | Activity Types                                                      | Event Types/Parsers                                                                                                                                                                                                                                                                                                                                                  | MITRE TTP                                                                                                                                                                              | Content                    |
|:-------------------------------------------------------------------:| ------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------- |
|    [Data Exfiltration](../UseCases/usecase_data_exfiltration.md)    | - Data Loss Prevention                                              |  dlp-alert<br> -- [safend-dlp-alert](../Parsers/parserContent_safend-dlp-alert.md)<br><br> usb-insert<br> -- [safend-usb-insert](../Parsers/parserContent_safend-usb-insert.md)<br><br> usb-read<br> -- [safend-usb-read](../Parsers/parserContent_safend-usb-read.md)<br><br> usb-write<br> -- [safend-usb-write](../Parsers/parserContent_safend-usb-write.md)<br> | T1020 - Automated Exfiltration<br>T1048 - Exfiltration Over Alternative Protocol<br>T1052.001 - Exfiltration Over Physical Medium: Exfiltration over USB<br>T1204 - User Execution<br> |  - 20 Rules<br> - 6 Models |
|    [Malware Detection](../UseCases/usecase_malware_detection.md)    | - Data Loss Prevention<br>- Endpoint Activity<br>- Process Activity |  dlp-alert<br> -- [safend-dlp-alert](../Parsers/parserContent_safend-dlp-alert.md)<br><br> usb-insert<br> -- [safend-usb-insert](../Parsers/parserContent_safend-usb-insert.md)<br><br> usb-read<br> -- [safend-usb-read](../Parsers/parserContent_safend-usb-read.md)<br><br> usb-write<br> -- [safend-usb-write](../Parsers/parserContent_safend-usb-write.md)<br> | T1204 - User Execution<br>                                                                                                                                                             |  - 5 Rules<br> - 1 Models  |
| [Ransomware Detection](../UseCases/usecase_ransomware_detection.md) | - Data Loss Prevention<br>- Endpoint Activity<br>- Process Activity |  dlp-alert<br> -- [safend-dlp-alert](../Parsers/parserContent_safend-dlp-alert.md)<br><br> usb-insert<br> -- [safend-usb-insert](../Parsers/parserContent_safend-usb-insert.md)<br><br> usb-read<br> -- [safend-usb-read](../Parsers/parserContent_safend-usb-read.md)<br><br> usb-write<br> -- [safend-usb-write](../Parsers/parserContent_safend-usb-write.md)<br> | T1204 - User Execution<br>                                                                                                                                                             |  - 5 Rules<br> - 1 Models  |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access | Execution                                                           | Persistence | Privilage escalation | Defense evasion | Credential Access | Discovery | Lateral Movement | Collection | Command and Control | Exfiltration                                                                                                                                                                                                                                                                                                                                                                  | Impact |
| -------------- | ------------------------------------------------------------------- | ----------- | -------------------- | --------------- | ----------------- | --------- | ---------------- | ---------- | ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------ |
|                | [User Execution](https://attack.mitre.org/techniques/T1204)<br><br> |             |                      |                 |                   |           |                  |            |                     | [Exfiltration Over Alternative Protocol](https://attack.mitre.org/techniques/T1048)<br><br>[Exfiltration Over Physical Medium: Exfiltration over USB](https://attack.mitre.org/techniques/T1052/001)<br><br>[Exfiltration Over Physical Medium](https://attack.mitre.org/techniques/T1052)<br><br>[Automated Exfiltration](https://attack.mitre.org/techniques/T1020)<br><br> |        |