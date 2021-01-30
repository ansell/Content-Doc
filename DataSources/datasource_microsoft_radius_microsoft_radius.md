Vendor: Microsoft Radius
========================
Product: Microsoft Radius
-------------------------
| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|   1   |   1    |     1      |      1      |    1    |

|               Use-Case                | Activity Types                            | Event Types/Parsers                                                                                         | MITRE TTP                  | Content                                             |
|:-------------------------------------:| ----------------------------------------- | ----------------------------------------------------------------------------------------------------------- | -------------------------- | --------------------------------------------------- |
| [Other](../UseCases/usecase_other.md) | <ul><li>Activity Time  and Type</li></ul> |  nac-logon<br> ↳ [s-radius-wireless-nac-logon](../Parsers/parserContent_s-radius-wireless-nac-logon.md)<br> | T1078 - Valid Accounts<br> | <ul><li>1 Rules</li></ul><ul><li>1 Models</li></ul> |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access                                                      | Execution | Persistence                                                         | Privilege Escalation                                                | Defense Evasion                                                     | Credential Access | Discovery | Lateral Movement | Collection | Command and Control | Exfiltration | Impact |
| ------------------------------------------------------------------- | --------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ----------------- | --------- | ---------------- | ---------- | ------------------- | ------------ | ------ |
| [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |           | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |                   |           |                  |            |                     |              |        |