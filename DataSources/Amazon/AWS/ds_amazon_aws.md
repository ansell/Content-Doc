Vendor: Amazon
==============
Product: AWS
------------
| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|  29   |   1    |     5      |      1      |    1    |

|                               Use-Case                               | Activity Types                                                 | Event Types/Parsers                                                                                                     | MITRE TTP                                                                                                    | Content                                                                          |
|:--------------------------------------------------------------------:| -------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------- |
|    [Data Exfiltration](../../../UseCases/uc_data_exfiltration.md)    | <ul><li>Netflow</li></ul>                                      |  netflow-connection<br> ↳ [cef-aws-vpc-netflow-connection](Parsers/parserContent_cef-aws-vpc-netflow-connection.md)<br> | T1048 - Exfiltration Over Alternative Protocol<br>                                                           | [<ul><li>1 Rules</li></ul>](Rules_Models/r_m_amazon_aws_Data_Exfiltration.md)    |
|     [Lateral Movement](../../../UseCases/uc_lateral_movement.md)     | <ul><li>Netflow</li><li>Network</li><li>Web Activity</li></ul> |  netflow-connection<br> ↳ [cef-aws-vpc-netflow-connection](Parsers/parserContent_cef-aws-vpc-netflow-connection.md)<br> | T1043 - T1043<br>T1046 - Network Service Scanning<br>T1065 - T1065<br>T1071 - Application Layer Protocol<br> | [<ul><li>25 Rules</li></ul>](Rules_Models/r_m_amazon_aws_Lateral_Movement.md)    |
|    [Malware Detection](../../../UseCases/uc_malware_detection.md)    | <ul><li>Network</li><li>Web Activity</li></ul>                 |  netflow-connection<br> ↳ [cef-aws-vpc-netflow-connection](Parsers/parserContent_cef-aws-vpc-netflow-connection.md)<br> | T1071 - Application Layer Protocol<br>                                                                       | [<ul><li>13 Rules</li></ul>](Rules_Models/r_m_amazon_aws_Malware_Detection.md)   |
|             [Phishing](../../../UseCases/uc_phishing.md)             | <ul><li>Network</li></ul>                                      |  netflow-connection<br> ↳ [cef-aws-vpc-netflow-connection](Parsers/parserContent_cef-aws-vpc-netflow-connection.md)<br> | T1071 - Application Layer Protocol<br>                                                                       | [<ul><li>1 Rules</li></ul>](Rules_Models/r_m_amazon_aws_Phishing.md)             |
| [Ransomware Detection](../../../UseCases/uc_ransomware_detection.md) | <ul><li>Network</li></ul>                                      |  netflow-connection<br> ↳ [cef-aws-vpc-netflow-connection](Parsers/parserContent_cef-aws-vpc-netflow-connection.md)<br> | T1071 - Application Layer Protocol<br>                                                                       | [<ul><li>3 Rules</li></ul>](Rules_Models/r_m_amazon_aws_Ransomware_Detection.md) |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access | Execution | Persistence | Privilege Escalation | Defense Evasion | Credential Access | Discovery                                                                     | Lateral Movement | Collection | Command and Control                                                             | Exfiltration                                                                                | Impact |
| -------------- | --------- | ----------- | -------------------- | --------------- | ----------------- | ----------------------------------------------------------------------------- | ---------------- | ---------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | ------ |
|                |           |             |                      |                 |                   | [Network Service Scanning](https://attack.mitre.org/techniques/T1046)<br><br> |                  |            | [Application Layer Protocol](https://attack.mitre.org/techniques/T1071)<br><br> | [Exfiltration Over Alternative Protocol](https://attack.mitre.org/techniques/T1048)<br><br> |        |