Vendor: IPswitch MoveIt
=======================
Product: IPswitch MoveIt
------------------------
| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|  63   |   10   |     6      |      5      |    5    |

|                                  Use-Case                                  | Activity Types                                                                                                                                                                                                                                                 | Event Types/Parsers                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | MITRE TTP                                                                                                                                                | Content                                                                                                                             |
|:--------------------------------------------------------------------------:| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| [Compromised Credentials](../../../UseCases/uc_compromised_credentials.md) | <ul><li>Activity Time  and Type</li><li>Application Activity</li><li>Asset Logon and Access</li><li>Critical System Activity</li><li>Email Activity</li><li>File Activity</li><li>Network zones and Location Access</li><li>Service Account Activity</li></ul> |  app-activity<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br><br> app-login<br> ↳ [cef-moveit-app-login](Parsers/parserContent_cef-moveit-app-login.md)<br><br> failed-app-login<br> ↳ [cef-moveit-app-failed-login](Parsers/parserContent_cef-moveit-app-failed-login.md)<br><br> file-read<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br><br> file-write<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br> | T1048 - Exfiltration Over Alternative Protocol<br>T1078 - Valid Accounts<br>T1083 - File and Directory Discovery<br>T1133 - External Remote Services<br> | [<ul><li>45 Rules</li></ul><ul><li>7 Models</li></ul>](Rules_Models/r_m_ipswitch_moveit_ipswitch_moveit_Compromised_Credentials.md) |
|       [Data Exfiltration](../../../UseCases/uc_data_exfiltration.md)       | <ul><li>Email Activity</li><li>File Activity</li></ul>                                                                                                                                                                                                         |  app-activity<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br><br> app-login<br> ↳ [cef-moveit-app-login](Parsers/parserContent_cef-moveit-app-login.md)<br><br> failed-app-login<br> ↳ [cef-moveit-app-failed-login](Parsers/parserContent_cef-moveit-app-failed-login.md)<br><br> file-read<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br><br> file-write<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br> | T1048 - Exfiltration Over Alternative Protocol<br>T1083 - File and Directory Discovery<br>                                                               | [<ul><li>5 Rules</li></ul><ul><li>2 Models</li></ul>](Rules_Models/r_m_ipswitch_moveit_ipswitch_moveit_Data_Exfiltration.md)        |
|         [Data Extraction](../../../UseCases/uc_data_extraction.md)         | <ul><li>File Activity</li></ul>                                                                                                                                                                                                                                |  app-activity<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br><br> app-login<br> ↳ [cef-moveit-app-login](Parsers/parserContent_cef-moveit-app-login.md)<br><br> failed-app-login<br> ↳ [cef-moveit-app-failed-login](Parsers/parserContent_cef-moveit-app-failed-login.md)<br><br> file-read<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br><br> file-write<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br> | T1083 - File and Directory Discovery<br>                                                                                                                 | [<ul><li>1 Rules</li></ul><ul><li>1 Models</li></ul>](Rules_Models/r_m_ipswitch_moveit_ipswitch_moveit_Data_Extraction.md)          |
|          [Internal Fraud](../../../UseCases/uc_internal_fraud.md)          | <ul><li>Application Activity</li></ul>                                                                                                                                                                                                                         |  app-activity<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br><br> app-login<br> ↳ [cef-moveit-app-login](Parsers/parserContent_cef-moveit-app-login.md)<br><br> failed-app-login<br> ↳ [cef-moveit-app-failed-login](Parsers/parserContent_cef-moveit-app-failed-login.md)<br><br> file-read<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br><br> file-write<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br> | T1078 - Valid Accounts<br>                                                                                                                               | [<ul><li>13 Rules</li></ul><ul><li>1 Models</li></ul>](Rules_Models/r_m_ipswitch_moveit_ipswitch_moveit_Internal_Fraud.md)          |
|        [Lateral Movement](../../../UseCases/uc_lateral_movement.md)        | <ul><li>Activity Time  and Type</li><li>Application Activity</li><li>Network zones and Location Access</li></ul>                                                                                                                                               |  app-activity<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br><br> app-login<br> ↳ [cef-moveit-app-login](Parsers/parserContent_cef-moveit-app-login.md)<br><br> failed-app-login<br> ↳ [cef-moveit-app-failed-login](Parsers/parserContent_cef-moveit-app-failed-login.md)<br><br> file-read<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br><br> file-write<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br> | T1078 - Valid Accounts<br>T1133 - External Remote Services<br>                                                                                           | [<ul><li>7 Rules</li></ul><ul><li>1 Models</li></ul>](Rules_Models/r_m_ipswitch_moveit_ipswitch_moveit_Lateral_Movement.md)         |
|       [Malware Detection](../../../UseCases/uc_malware_detection.md)       | <ul><li>Asset Logon and Access</li><li>Endpoint Activity</li><li>File Activity</li></ul>                                                                                                                                                                       |  app-activity<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br><br> app-login<br> ↳ [cef-moveit-app-login](Parsers/parserContent_cef-moveit-app-login.md)<br><br> failed-app-login<br> ↳ [cef-moveit-app-failed-login](Parsers/parserContent_cef-moveit-app-failed-login.md)<br><br> file-read<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br><br> file-write<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br> | T1188 - T1188<br>T1204 - User Execution<br>                                                                                                              | [<ul><li>9 Rules</li></ul><ul><li>1 Models</li></ul>](Rules_Models/r_m_ipswitch_moveit_ipswitch_moveit_Malware_Detection.md)        |
|     [Privileged Activity](../../../UseCases/uc_privileged_activity.md)     | <ul><li>Application Activity</li><li>Email Activity</li><li>Service Account Activity</li></ul>                                                                                                                                                                 |  app-activity<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br><br> app-login<br> ↳ [cef-moveit-app-login](Parsers/parserContent_cef-moveit-app-login.md)<br><br> failed-app-login<br> ↳ [cef-moveit-app-failed-login](Parsers/parserContent_cef-moveit-app-failed-login.md)<br><br> file-read<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br><br> file-write<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br> | T1048 - Exfiltration Over Alternative Protocol<br>T1078 - Valid Accounts<br>                                                                             | [<ul><li>5 Rules</li></ul><ul><li>1 Models</li></ul>](Rules_Models/r_m_ipswitch_moveit_ipswitch_moveit_Privileged_Activity.md)      |
|    [Ransomware Detection](../../../UseCases/uc_ransomware_detection.md)    | <ul><li>Asset Logon and Access</li><li>Endpoint Activity</li><li>File Activity</li></ul>                                                                                                                                                                       |  app-activity<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br><br> app-login<br> ↳ [cef-moveit-app-login](Parsers/parserContent_cef-moveit-app-login.md)<br><br> failed-app-login<br> ↳ [cef-moveit-app-failed-login](Parsers/parserContent_cef-moveit-app-failed-login.md)<br><br> file-read<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br><br> file-write<br> ↳ [cef-moveit-activity](Parsers/parserContent_cef-moveit-activity.md)<br> | T1188 - T1188<br>T1204 - User Execution<br>                                                                                                              | [<ul><li>9 Rules</li></ul><ul><li>1 Models</li></ul>](Rules_Models/r_m_ipswitch_moveit_ipswitch_moveit_Ransomware_Detection.md)     |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access                                                                                                                                   | Execution                                                           | Persistence                                                                                                                                      | Privilege Escalation                                                | Defense Evasion                                                     | Credential Access | Discovery                                                                         | Lateral Movement | Collection | Command and Control | Exfiltration                                                                                | Impact |
| ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ----------------- | --------------------------------------------------------------------------------- | ---------------- | ---------- | ------------------- | ------------------------------------------------------------------------------------------- | ------ |
| [External Remote Services](https://attack.mitre.org/techniques/T1133)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [User Execution](https://attack.mitre.org/techniques/T1204)<br><br> | [External Remote Services](https://attack.mitre.org/techniques/T1133)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |                   | [File and Directory Discovery](https://attack.mitre.org/techniques/T1083)<br><br> |                  |            |                     | [Exfiltration Over Alternative Protocol](https://attack.mitre.org/techniques/T1048)<br><br> |        |