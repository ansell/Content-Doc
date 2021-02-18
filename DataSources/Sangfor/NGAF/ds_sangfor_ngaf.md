Vendor: Sangfor
===============
Product: NGAF
-------------
| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|  67   |   13   |     12     |      3      |    3    |

|                                  Use-Case                                  | Activity Types                                                                                    | Event Types/Parsers                                                                                                                                                                                                                                                                                               | MITRE TTP                                                                                                                                                                                                                                                                                                                                                                              | Content                                                                                                          |
|:--------------------------------------------------------------------------:| ------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| [Compromised Credentials](../../../UseCases/uc_compromised_credentials.md) | <ul><li>Web Activity</li></ul>                                                                    |  network-alert<br> ↳ [sangfor-network-alert](Parsers/parserContent_sangfor-network-alert.md)<br><br> web-activity-allowed<br> ↳ [sangfor-web-activity](Parsers/parserContent_sangfor-web-activity.md)<br><br> web-activity-denied<br> ↳ [sangfor-web-activity](Parsers/parserContent_sangfor-web-activity.md)<br> | T1071.001 - Application Layer Protocol: Web Protocols<br>                                                                                                                                                                                                                                                                                                                              | [<ul><li>11 Rules</li></ul><ul><li>1 Models</li></ul>](Rules_Models/r_m_sangfor_ngaf_Compromised_Credentials.md) |
|       [Data Exfiltration](../../../UseCases/uc_data_exfiltration.md)       | <ul><li>Data Loss Prevention</li><li>Web Activity</li></ul>                                       |  network-alert<br> ↳ [sangfor-network-alert](Parsers/parserContent_sangfor-network-alert.md)<br><br> web-activity-allowed<br> ↳ [sangfor-web-activity](Parsers/parserContent_sangfor-web-activity.md)<br><br> web-activity-denied<br> ↳ [sangfor-web-activity](Parsers/parserContent_sangfor-web-activity.md)<br> | T1030 - Data Transfer Size Limits<br>T1071.001 - Application Layer Protocol: Web Protocols<br>T1567.002 - Exfiltration Over Web Service: Exfiltration to Cloud Storage<br>                                                                                                                                                                                                             | [<ul><li>3 Rules</li></ul>](Rules_Models/r_m_sangfor_ngaf_Data_Exfiltration.md)                                  |
|          [Internal Fraud](../../../UseCases/uc_internal_fraud.md)          | <ul><li>Web Activity</li></ul>                                                                    |  network-alert<br> ↳ [sangfor-network-alert](Parsers/parserContent_sangfor-network-alert.md)<br><br> web-activity-allowed<br> ↳ [sangfor-web-activity](Parsers/parserContent_sangfor-web-activity.md)<br><br> web-activity-denied<br> ↳ [sangfor-web-activity](Parsers/parserContent_sangfor-web-activity.md)<br> | T1071.001 - Application Layer Protocol: Web Protocols<br>                                                                                                                                                                                                                                                                                                                              | [<ul><li>3 Rules</li></ul><ul><li>2 Models</li></ul>](Rules_Models/r_m_sangfor_ngaf_Internal_Fraud.md)           |
|        [Lateral Movement](../../../UseCases/uc_lateral_movement.md)        | <ul><li>Network Alert</li><li>Security Alert</li><li>Web Activity</li></ul>                       |  network-alert<br> ↳ [sangfor-network-alert](Parsers/parserContent_sangfor-network-alert.md)<br><br> web-activity-allowed<br> ↳ [sangfor-web-activity](Parsers/parserContent_sangfor-web-activity.md)<br><br> web-activity-denied<br> ↳ [sangfor-web-activity](Parsers/parserContent_sangfor-web-activity.md)<br> | T1027.005 - Obfuscated Files or Information: Indicator Removal from Tools<br>T1071 - Application Layer Protocol<br>T1071.001 - Application Layer Protocol: Web Protocols<br>                                                                                                                                                                                                           | [<ul><li>10 Rules</li></ul><ul><li>6 Models</li></ul>](Rules_Models/r_m_sangfor_ngaf_Lateral_Movement.md)        |
|       [Malware Detection](../../../UseCases/uc_malware_detection.md)       | <ul><li>Endpoint Activity</li><li>Network</li><li>Process Activity</li><li>Web Activity</li></ul> |  network-alert<br> ↳ [sangfor-network-alert](Parsers/parserContent_sangfor-network-alert.md)<br><br> web-activity-allowed<br> ↳ [sangfor-web-activity](Parsers/parserContent_sangfor-web-activity.md)<br><br> web-activity-denied<br> ↳ [sangfor-web-activity](Parsers/parserContent_sangfor-web-activity.md)<br> | T1071 - Application Layer Protocol<br>T1071.001 - Application Layer Protocol: Web Protocols<br>T1090.003 - Proxy: Multi-hop Proxy<br>T1102 - Web Service<br>T1204 - User Execution<br>T1496 - Resource Hijacking<br>T1550.002 - Use Alternate Authentication Material: Pass the Hash<br>T1568 - Dynamic Resolution<br>T1568.002 - Dynamic Resolution: Domain Generation Algorithms<br> | [<ul><li>43 Rules</li></ul><ul><li>5 Models</li></ul>](Rules_Models/r_m_sangfor_ngaf_Malware_Detection.md)       |
|                [Phishing](../../../UseCases/uc_phishing.md)                | <ul><li>Network</li><li>Web Activity</li></ul>                                                    |  network-alert<br> ↳ [sangfor-network-alert](Parsers/parserContent_sangfor-network-alert.md)<br><br> web-activity-allowed<br> ↳ [sangfor-web-activity](Parsers/parserContent_sangfor-web-activity.md)<br><br> web-activity-denied<br> ↳ [sangfor-web-activity](Parsers/parserContent_sangfor-web-activity.md)<br> | T1071 - Application Layer Protocol<br>T1071.001 - Application Layer Protocol: Web Protocols<br>T1566.002 - Phishing: Spearphishing Link<br>T1568 - Dynamic Resolution<br>                                                                                                                                                                                                              | [<ul><li>8 Rules</li></ul>](Rules_Models/r_m_sangfor_ngaf_Phishing.md)                                           |
|    [Ransomware Detection](../../../UseCases/uc_ransomware_detection.md)    | <ul><li>Endpoint Activity</li><li>Network</li><li>Process Activity</li><li>Web Activity</li></ul> |  network-alert<br> ↳ [sangfor-network-alert](Parsers/parserContent_sangfor-network-alert.md)<br><br> web-activity-allowed<br> ↳ [sangfor-web-activity](Parsers/parserContent_sangfor-web-activity.md)<br><br> web-activity-denied<br> ↳ [sangfor-web-activity](Parsers/parserContent_sangfor-web-activity.md)<br> | T1071 - Application Layer Protocol<br>T1071.001 - Application Layer Protocol: Web Protocols<br>T1090.003 - Proxy: Multi-hop Proxy<br>T1102 - Web Service<br>T1204 - User Execution<br>T1496 - Resource Hijacking<br>T1550.002 - Use Alternate Authentication Material: Pass the Hash<br>T1568 - Dynamic Resolution<br>T1568.002 - Dynamic Resolution: Domain Generation Algorithms<br> | [<ul><li>40 Rules</li></ul><ul><li>4 Models</li></ul>](Rules_Models/r_m_sangfor_ngaf_Ransomware_Detection.md)    |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access                                                                                                                                     | Execution                                                           | Persistence | Privilege Escalation | Defense Evasion                                                                                                                                                                                                                                                                                                                                                                                                   | Credential Access | Discovery | Lateral Movement                                                                           | Collection | Command and Control                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        | Exfiltration                                                                                                                                                                                                                                                                          | Impact                                                                  |
| -------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- | ----------- | -------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------- | --------- | ------------------------------------------------------------------------------------------ | ---------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| [Phishing: Spearphishing Link](https://attack.mitre.org/techniques/T1566/002)<br><br>[Phishing](https://attack.mitre.org/techniques/T1566)<br><br> | [User Execution](https://attack.mitre.org/techniques/T1204)<br><br> |             |                      | [Obfuscated Files or Information: Indicator Removal from Tools](https://attack.mitre.org/techniques/T1027/005)<br><br>[Use Alternate Authentication Material](https://attack.mitre.org/techniques/T1550)<br><br>[Use Alternate Authentication Material: Pass the Hash](https://attack.mitre.org/techniques/T1550/002)<br><br>[Obfuscated Files or Information](https://attack.mitre.org/techniques/T1027)<br><br> |                   |           | [Use Alternate Authentication Material](https://attack.mitre.org/techniques/T1550)<br><br> |            | [Web Service](https://attack.mitre.org/techniques/T1102)<br><br>[Application Layer Protocol: Web Protocols](https://attack.mitre.org/techniques/T1071/001)<br><br>[Dynamic Resolution](https://attack.mitre.org/techniques/T1568)<br><br>[Dynamic Resolution: Domain Generation Algorithms](https://attack.mitre.org/techniques/T1568/002)<br><br>[Proxy: Multi-hop Proxy](https://attack.mitre.org/techniques/T1090/003)<br><br>[Application Layer Protocol](https://attack.mitre.org/techniques/T1071)<br><br>[Proxy](https://attack.mitre.org/techniques/T1090)<br><br> | [Data Transfer Size Limits](https://attack.mitre.org/techniques/T1030)<br><br>[Exfiltration Over Web Service: Exfiltration to Cloud Storage](https://attack.mitre.org/techniques/T1567/002)<br><br>[Exfiltration Over Web Service](https://attack.mitre.org/techniques/T1567)<br><br> | [Resource Hijacking](https://attack.mitre.org/techniques/T1496)<br><br> |