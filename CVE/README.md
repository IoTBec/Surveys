# CVE Survey Overview

Between **May 26 and May 29, 2025 (Beijing Time)**, we surveyed all CVE IDs of **Tenda**, **TOTOLINK**, **D-Link**, and **TP-Link**, along with their corresponding CNA organizations. The statistical distribution is shown in [Fig1](https://raw.githubusercontent.com/abcdefg-png/images2/main/image-20250809120518088.png).

![image-20250809120518088](https://raw.githubusercontent.com/abcdefg-png/images2/main/image-20250809120518088.png)

From the full CVE set, we randomly sampled **125** CVE IDs for each vendor (**500** in total, with **60%** from 2023 and earlier, and **40%** from 2024~2025). We manually verified whether the CVE **Descriptions** and their **Reference** reports contained the two key information required for IoTBec's Vulnerability Signature construction:

- **Affected `POST Interface`**
- **`Critical parameter`**

The survey results are summarized below.

|  Vendor  |      Year       | Interface&parameter in  Reference | Interface&parameter in  Description | Interface&parameter in  Reference or Description |
| :------: | :-------------: | :-------------------------------: | :---------------------------------: | :----------------------------------------------: |
|  Tenda   | 2023 or earlier |               39/75               |                20/75                |                    47/75=63%                     |
|          |    2024~2025    |               40/50               |                29/50                |                    46/50=92%                     |
| TOTOLINK | 2023 or earlier |               45/75               |                21/75                |                    51/75=68%                     |
|          |    2024~2025    |               34/50               |                29/50                |                    45/50=90%                     |
|  D-Link  | 2023 or earlier |               19/75               |                32/75                |                    38/75=51%                     |
|          |    2024~2025    |               37/50               |                29/50                |                    39/50=78%                     |
| TP-Link  | 2023 or earlier |               34/75               |                25/75                |                    49/75=65%                     |
|          |    2024~2025    |               25/50               |                19/50                |                    37/50=74%                     |

2023 or  earlier: 185/300≈62%; 2024~2025: 167/200≈**84%**

Notably, as shown in [Fig1](https://raw.githubusercontent.com/abcdefg-png/images2/main/image-20250809120518088.png), since 2024, the proportion of IoT-related CVEs issued by CNA VULDB has surged dramatically. Among the **88** CVE IDs issued by **VULDB** (out of the total 500), **82** contained both key information, representing approximately **93.2%** coverage.

|  Vendor  |      Year       | Interface&parameter by in Reference VULDB | Interface&parameter in  Description by VULDB | Interface&parameter in  Reference or Description by VULDB |
| :------: | :-------------: | :---------------------------------------: | :------------------------------------------: | :-------------------------------------------------------: |
|  Tenda   | 2023 or earlier |                    0/1                    |                     0/1                      |                          0/1=0%                           |
|          |    2024~2025    |                   17/20                   |                    18/20                     |                        20/20=100%                         |
| TOTOLINK | 2023 or earlier |                    1/3                    |                     2/3                      |                          2/3=66%                          |
|          |    2024~2025    |                   14/27                   |                    26/27                     |                         26/27=96%                         |
|  D-Link  | 2023 or earlier |                    1/1                    |                     1/1                      |                         1/1=100%                          |
|          |    2024~2025    |                   25/30                   |                    25/30                     |                         27/30=90%                         |
| TP-Link  | 2023 or earlier |                    1/1                    |                     0/0                      |                         1/1=100%                          |
|          |    2024~2025    |                    5/5                    |                     3/5                      |                         5/5=100%                          |

2023 or  earlier: 4/6≈66%; 2024~2025: 78/82≈**95%**
