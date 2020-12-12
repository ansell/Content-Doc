Vendor: Ping Identity
=====================
Product: PingID
---------------
|                                 Use-Case                                  | Activity Types                                                   | Event Types/Parsers                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | MITRE TTP                                                        | Content                   |
|:-------------------------------------------------------------------------:| ---------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- | ------------------------- |
| [Compromised Credentials](../UseCases/usecase_compromised_credentials.md) | - Activity Time  and Type<br>- Network zones and Location Access |  account-password-change<br> -- [cef-pingid-auth](../Parsers/parserContent_cef-pingid-auth.md)<br><br> account-password-change-failed<br> -- [cef-pingid-auth](../Parsers/parserContent_cef-pingid-auth.md)<br><br> account-password-reset<br> -- [cef-pingid-auth](../Parsers/parserContent_cef-pingid-auth.md)<br><br> authentication-failed<br> -- [cef-pingid-auth](../Parsers/parserContent_cef-pingid-auth.md)<br><br> authentication-successful<br> -- [cef-pingid-auth](../Parsers/parserContent_cef-pingid-auth.md)<br> | T1078 - Valid Accounts<br>T1133 - External Remote Services<br>   |  - 9 Rules<br> - 4 Models |
|        [Lateral Movement](../UseCases/usecase_lateral_movement.md)        | - Network zones and Location Access                              |  account-password-change<br> -- [cef-pingid-auth](../Parsers/parserContent_cef-pingid-auth.md)<br><br> account-password-change-failed<br> -- [cef-pingid-auth](../Parsers/parserContent_cef-pingid-auth.md)<br><br> account-password-reset<br> -- [cef-pingid-auth](../Parsers/parserContent_cef-pingid-auth.md)<br><br> authentication-failed<br> -- [cef-pingid-auth](../Parsers/parserContent_cef-pingid-auth.md)<br><br> authentication-successful<br> -- [cef-pingid-auth](../Parsers/parserContent_cef-pingid-auth.md)<br> | T1078 - Valid Accounts<br>T1133 - External Remote Services<br>   |  - 2 Rules<br> - 1 Models |
|       [Malware Detection](../UseCases/usecase_malware_detection.md)       | - Asset Logon and Access                                         |  account-password-change<br> -- [cef-pingid-auth](../Parsers/parserContent_cef-pingid-auth.md)<br><br> account-password-change-failed<br> -- [cef-pingid-auth](../Parsers/parserContent_cef-pingid-auth.md)<br><br> account-password-reset<br> -- [cef-pingid-auth](../Parsers/parserContent_cef-pingid-auth.md)<br><br> authentication-failed<br> -- [cef-pingid-auth](../Parsers/parserContent_cef-pingid-auth.md)<br><br> authentication-successful<br> -- [cef-pingid-auth](../Parsers/parserContent_cef-pingid-auth.md)<br> | T1078 - Valid Accounts<br>T1090.003 - Proxy: Multi-hop Proxy<br> |  - 6 Rules<br>            |
|    [Ransomware Detection](../UseCases/usecase_ransomware_detection.md)    | - Asset Logon and Access                                         |  account-password-change<br> -- [cef-pingid-auth](../Parsers/parserContent_cef-pingid-auth.md)<br><br> account-password-change-failed<br> -- [cef-pingid-auth](../Parsers/parserContent_cef-pingid-auth.md)<br><br> account-password-reset<br> -- [cef-pingid-auth](../Parsers/parserContent_cef-pingid-auth.md)<br><br> authentication-failed<br> -- [cef-pingid-auth](../Parsers/parserContent_cef-pingid-auth.md)<br><br> authentication-successful<br> -- [cef-pingid-auth](../Parsers/parserContent_cef-pingid-auth.md)<br> | T1078 - Valid Accounts<br>T1090.003 - Proxy: Multi-hop Proxy<br> |  - 6 Rules<br>            |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access                                                                                                                                   | Execution | Persistence                                                                                                                                      | Privilage escalation                                                | Defense evasion                                                     | Credential Access | Discovery | Lateral Movement | Collection | Command and Control                                                                                                                       | Exfiltration | Impact |
| ------------------------------------------------------------------------------------------------------------------------------------------------ | --------- | ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ----------------- | --------- | ---------------- | ---------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ------------ | ------ |
| [External Remote Services](https://attack.mitre.org/techniques/T1133)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |           | [External Remote Services](https://attack.mitre.org/techniques/T1133)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |                   |           |                  |            | [Proxy: Multi-hop Proxy](https://attack.mitre.org/techniques/T1090/003)<br><br>[Proxy](https://attack.mitre.org/techniques/T1090)<br><br> |              |        |