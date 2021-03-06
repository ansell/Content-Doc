Vendor: Check Point Software
============================
### Product: [Check Point Identity Awareness](../ds_check_point_software_check_point_identity_awareness.md)
### Use-Case: [Phishing](../../../../UseCases/uc_phishing.md)

| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|   3   |   1    |     2      |      4      |    4    |

| Event Type                    | Rules                                                                                                                                                                                                        | Models |
| ----------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------ |
| network-connection-failed     | <b>T1071 - Application Layer Protocol</b><br> ↳ <b>NETF-TI-IP-Outbound</b>: Outbound failed connection to a known malicious IP<br> ↳ <b>NET-TI-H-Outbound</b>: Outbound connection to a known malicious host |        |
| network-connection-successful | <b>T1071 - Application Layer Protocol</b><br> ↳ <b>NET-TI-H-Outbound</b>: Outbound connection to a known malicious host                                                                                      |        |
| vpn-logout                    | <b>T1566 - Phishing</b><br> ↳ <b>EM-BSum-in</b>: Abnormal size of incoming emails                                                                                                                            |        |