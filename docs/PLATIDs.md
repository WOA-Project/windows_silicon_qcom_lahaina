# ACPI Platform Identifiers

## Snapdragon 888

### ATP

| ACPI _SUB String (Subsystem/Platform ID) | Matching SOID (SoC ID) | Matching PLST (Platform Subtype) | Friendly Name      |
|------------------------------------------|------------------------|----------------------------------|--------------------|
| ATP08350                                 | 415, 456, 501          | 0                                | MSM™               |
| ATPA8350                                 | 439, 502               | 0                                | APQ™               |

### CDP

| ACPI _SUB String (Subsystem/Platform ID) | Matching SOID (SoC ID) | Matching PLST (Platform Subtype) | Friendly Name      |
|------------------------------------------|------------------------|----------------------------------|--------------------|
| CDP08350                                 | 415, 456, 501          | 0                                | MSM™               |
| CDP18350                                 | 415, 456, 501          | 3                                | MSM™ + HSP PRO     |
| CDPA8350                                 | 439, 502               | 0                                | APQ™               |

### HDK

| ACPI _SUB String (Subsystem/Platform ID) | Matching SOID (SoC ID) | Matching PLST (Platform Subtype) | Friendly Name      |
|------------------------------------------|------------------------|----------------------------------|--------------------|
| HDK08350                                 | 415, 456, 501          | 0                                | MSM™               |
| HHG08350                                 | 415, 456, 501          | 1                                | MSM™               |
| HHGA8350                                 | 439, 502               | 2                                | APQ™ + HSP PRO     |

*HHG: Handheld Gaming Reference Device

### MTP

| ACPI _SUB String (Subsystem/Platform ID) | Matching SOID (SoC ID) | Matching PLST (Platform Subtype) | Friendly Name      |
|------------------------------------------|------------------------|----------------------------------|--------------------|
| MTP08350                                 | 415, 456, 501          | 0                                | MSM™               |
| MTP18350                                 | 415, 456, 501          | 1                                | MSM™ + HSP         |
| MTP28350                                 | 415, 456, 501          | 2                                | MSM™ + HSP PRO     |
| MTPA8350                                 | 439, 502               | 0                                | APQ™               |

### QRD

| ACPI _SUB String (Subsystem/Platform ID) | Matching SOID (SoC ID) | Matching PLST (Platform Subtype) | Friendly Name      |
|------------------------------------------|------------------------|----------------------------------|--------------------|
| QRD08350                                 | 415, 456, 501          | 0                                | MSM™               |
| QRD18350                                 | 415, 456, 501          | 1                                | MSM™ + HSP         |
| QRD28350                                 | 415, 456, 501          | 2                                | MSM™ + HSP PRO     |
| QSP08350                                 | 415, 456, 501          | 8                                | MSM™               |
| QRDA8350                                 | 439, 502               | 0                                | APQ™               |

*QSP: System In Package Module Reference Card

### RUMI

| ACPI _SUB String (Subsystem/Platform ID) | Matching SOID (SoC ID) | Matching PLST (Platform Subtype) | Friendly Name      |
|------------------------------------------|------------------------|----------------------------------|--------------------|
| RUMI8350                                 | 415, 456, 501          | 0                                | MSM™               |

# Device Tree Platform Identifiers

## Snapdragon 888

### ATP

| Device Tree Source File Name           | Matching ACPI Condition (Against header values prefilled from SMEM) |
|----------------------------------------|---------------------------------------------------------------------|
lahaina-atp-overlay.dts                  | Lequal(\\\_SB_.PSUB, "ATP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-atp.dts                          | Lequal(\\\_SB_.PSUB, "ATP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-v2-atp.dts                       | Lequal(\\\_SB_.PSUB, "ATP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-v2.1-atp.dts                     | Lequal(\\\_SB_.PSUB, "ATP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahainap-atp-overlay.dts                 | Lequal(\\\_SB_.PSUB, "ATP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahainap-atp.dts                         | Lequal(\\\_SB_.PSUB, "ATP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahainap-v2-atp.dts                      | Lequal(\\\_SB_.PSUB, "ATP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahainap-v2.1-atp.dts                    | Lequal(\\\_SB_.PSUB, "ATP08350") && Lequal(\\\_SB_.PLST, 0)         |

### RUMI

| Device Tree Source File Name           | Matching ACPI Condition (Against header values prefilled from SMEM) |
|----------------------------------------|---------------------------------------------------------------------|
lahaina-rumi-overlay.dts                 | Lequal(\\\_SB_.PSUB, "RUMI8350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-rumi.dts                         | Lequal(\\\_SB_.PSUB, "RUMI8350") && Lequal(\\\_SB_.PLST, 0)         |

### HDK

| Device Tree Source File Name           | Matching ACPI Condition (Against header values prefilled from SMEM) |
|----------------------------------------|---------------------------------------------------------------------|
lahaina-hdk-overlay.dts                  | Lequal(\\\_SB_.PSUB, "HDK08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-hdk.dts                          | Lequal(\\\_SB_.PSUB, "HDK08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-v2-hdk.dts                       | Lequal(\\\_SB_.PSUB, "HDK08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-v2.1-hdk.dts                     | Lequal(\\\_SB_.PSUB, "HDK08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-hhg-overlay.dts                  | Lequal(\\\_SB_.PSUB, "HDK08350") && Lequal(\\\_SB_.PLST, 1)         |
lahaina-v2.1-hhg.dts                     | Lequal(\\\_SB_.PSUB, "HDK08350") && Lequal(\\\_SB_.PLST, 1)         |
lahainap-hhg-hsp-pro-overlay.dts         | Lequal(\\\_SB_.PSUB, "HDK08350") && Lequal(\\\_SB_.PLST, 2)         |
lahainap-v2.1-hhg-hsp-pro.dts            | Lequal(\\\_SB_.PSUB, "HDK08350") && Lequal(\\\_SB_.PLST, 2)         |

### CDP

| Device Tree Source File Name           | Matching ACPI Condition (Against header values prefilled from SMEM) |
|----------------------------------------|---------------------------------------------------------------------|
lahaina-cdp-overlay.dts                  | Lequal(\\\_SB_.PSUB, "CDP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-cdp-v2.2-overlay.dts             | Lequal(\\\_SB_.PSUB, "CDP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-cdp-v2.2.dts                     | Lequal(\\\_SB_.PSUB, "CDP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-cdp.dts                          | Lequal(\\\_SB_.PSUB, "CDP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-v2-cdp.dts                       | Lequal(\\\_SB_.PSUB, "CDP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-v2.1-cdp.dts                     | Lequal(\\\_SB_.PSUB, "CDP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-vm-cdp.dts                       | Lequal(\\\_SB_.PSUB, "CDP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahainap-cdp-overlay.dts                 | Lequal(\\\_SB_.PSUB, "CDP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahainap-cdp.dts                         | Lequal(\\\_SB_.PSUB, "CDP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahainap-v2-cdp.dts                      | Lequal(\\\_SB_.PSUB, "CDP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahainap-v2.1-cdp.dts                    | Lequal(\\\_SB_.PSUB, "CDP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-v2.1-cdp-hsp-pro.dts             | Lequal(\\\_SB_.PSUB, "CDP08350") && Lequal(\\\_SB_.PLST, 3)         |
lahaina-cdp-hsp-pro-overlay.dts          | Lequal(\\\_SB_.PSUB, "CDP08350") && Lequal(\\\_SB_.PLST, 3)         |

### MTP

| Device Tree Source File Name           | Matching ACPI Condition (Against header values prefilled from SMEM) |
|----------------------------------------|---------------------------------------------------------------------|
lahaina-mtp-overlay.dts                  | Lequal(\\\_SB_.PSUB, "MTP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-mtp-v2-overlay.dts               | Lequal(\\\_SB_.PSUB, "MTP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-mtp-v2.1-overlay.dts             | Lequal(\\\_SB_.PSUB, "MTP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-mtp-v2.1.dts                     | Lequal(\\\_SB_.PSUB, "MTP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-mtp-v2.dts                       | Lequal(\\\_SB_.PSUB, "MTP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-mtp.dts                          | Lequal(\\\_SB_.PSUB, "MTP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-v2-mtp.dts                       | Lequal(\\\_SB_.PSUB, "MTP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-v2.1-mtp.dts                     | Lequal(\\\_SB_.PSUB, "MTP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-vm-mtp-v2.1.dts                  | Lequal(\\\_SB_.PSUB, "MTP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-vm-mtp-v2.dts                    | Lequal(\\\_SB_.PSUB, "MTP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-vm-mtp.dts                       | Lequal(\\\_SB_.PSUB, "MTP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahainap-mtp-overlay.dts                 | Lequal(\\\_SB_.PSUB, "MTP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahainap-mtp.dts                         | Lequal(\\\_SB_.PSUB, "MTP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahainap-v2-mtp.dts                      | Lequal(\\\_SB_.PSUB, "MTP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahainap-v2.1-mtp.dts                    | Lequal(\\\_SB_.PSUB, "MTP08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-mtp-hsp-overlay.dts              | Lequal(\\\_SB_.PSUB, "MTP08350") && Lequal(\\\_SB_.PLST, 1)         |
lahaina-mtp-hsp.dts                      | Lequal(\\\_SB_.PSUB, "MTP08350") && Lequal(\\\_SB_.PLST, 1)         |
lahaina-mtp-hsp-pro-overlay.dts          | Lequal(\\\_SB_.PSUB, "MTP08350") && Lequal(\\\_SB_.PLST, 2)         |
lahaina-v2.1-mtp-hsp-pro.dts             | Lequal(\\\_SB_.PSUB, "MTP08350") && Lequal(\\\_SB_.PLST, 2)         |

### QRD

| Device Tree Source File Name           | Matching ACPI Condition (Against header values prefilled from SMEM) |
|----------------------------------------|---------------------------------------------------------------------|
lahaina-qrd-overlay.dts                  | Lequal(\\\_SB_.PSUB, "QRD08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-qrd.dts                          | Lequal(\\\_SB_.PSUB, "QRD08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-v2-qrd.dts                       | Lequal(\\\_SB_.PSUB, "QRD08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-v2.1-qrd.dts                     | Lequal(\\\_SB_.PSUB, "QRD08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-vm-qrd.dts                       | Lequal(\\\_SB_.PSUB, "QRD08350") && Lequal(\\\_SB_.PLST, 0)         |
lahainap-qrd-overlay.dts                 | Lequal(\\\_SB_.PSUB, "QRD08350") && Lequal(\\\_SB_.PLST, 0)         |
lahainap-qrd.dts                         | Lequal(\\\_SB_.PSUB, "QRD08350") && Lequal(\\\_SB_.PLST, 0)         |
lahainap-v2-qrd.dts                      | Lequal(\\\_SB_.PSUB, "QRD08350") && Lequal(\\\_SB_.PLST, 0)         |
lahainap-v2.1-qrd.dts                    | Lequal(\\\_SB_.PSUB, "QRD08350") && Lequal(\\\_SB_.PLST, 0)         |
lahaina-qrd-hsp-overlay.dts              | Lequal(\\\_SB_.PSUB, "QRD08350") && Lequal(\\\_SB_.PLST, 1)         |
lahaina-qrd-hsp.dts                      | Lequal(\\\_SB_.PSUB, "QRD08350") && Lequal(\\\_SB_.PLST, 1)         |
lahaina-qrd-hsp-pro-overlay.dts          | Lequal(\\\_SB_.PSUB, "QRD08350") && Lequal(\\\_SB_.PLST, 2)         |
lahaina-v2.1-qrd-hsp-pro.dts             | Lequal(\\\_SB_.PSUB, "QRD08350") && Lequal(\\\_SB_.PLST, 2)         |
lahaina-qrd-module-overlay.dts           | Lequal(\\\_SB_.PSUB, "QRD08350") && Lequal(\\\_SB_.PLST, 8)         |
lahaina-qrd-module.dts                   | Lequal(\\\_SB_.PSUB, "QRD08350") && Lequal(\\\_SB_.PLST, 8)         |
lahaina-v2-qrd-module.dts                | Lequal(\\\_SB_.PSUB, "QRD08350") && Lequal(\\\_SB_.PLST, 8)         |
lahaina-v2.1-qrd-module.dts              | Lequal(\\\_SB_.PSUB, "QRD08350") && Lequal(\\\_SB_.PLST, 8)         |

---

## Snapdragon 888 (MSM)

| Device Tree Source File Name | Chip ID                        | Foundry ID | Reserved | PlatformID | RevID         |
|------------------------------|--------------------------------|------------|----------|------------|---------------|
| lahaina.dtsi                 | SM_LAHAINA (415)               | 0          | 0        | 0          | 1.0 (0x10000) |
| lahaina-vm.dtsi              | SM_LAHAINA (415)               | 0          | 0        | 0          | 1.0 (0x10000) |
| lahaina-v2.dtsi              | SM_LAHAINA (415)               | 0          | 0        | 0          | 2.0 (0x20000) |
| lahaina-vm-v2.dtsi           | SM_LAHAINA (415)               | 0          | 0        | 0          | 2.0 (0x20000) |
| lahaina-v2.1.dtsi            | SM_LAHAINA (415)               | 0          | 0        | 0          | 2.1 (0x20001) |
| lahaina.dtsi                 | SM_LAHAINA_MODULE (456)        | 0          | 0        | 0          | 1.0 (0x10000) |
| lahaina-v2.dtsi              | SM_LAHAINA_MODULE (456)        | 0          | 0        | 0          | 2.0 (0x20000) |
| lahaina-v2.1.dtsi            | SM_LAHAINA_MODULE (456)        | 0          | 0        | 0          | 2.1 (0x20001) |
| lahaina.dtsi                 | SM_LAHAINA_LTE_ONLY (501)      | 0          | 0        | 0          | 1.0 (0x10000) |
| lahaina-vm.dtsi              | SM_LAHAINA_LTE_ONLY (501)      | 0          | 0        | 0          | 1.0 (0x10000) |
| lahaina-v2.dtsi              | SM_LAHAINA_LTE_ONLY (501)      | 0          | 0        | 0          | 2.0 (0x20000) |
| lahaina-vm-v2.dtsi           | SM_LAHAINA_LTE_ONLY (501)      | 0          | 0        | 0          | 2.0 (0x20000) |
| lahaina-v2.1.dtsi            | SM_LAHAINA_LTE_ONLY (501)      | 0          | 0        | 0          | 2.1 (0x20001) |

## Snapdragon 888 (APQ)

| Device Tree Source File Name | Chip ID                        | Foundry ID | Reserved | PlatformID | RevID         |
|------------------------------|--------------------------------|------------|----------|------------|---------------|
| lahainap.dtsi                | SMP_LAHAINA (439)              | 0          | 0        | 0          | 1.0 (0x10000) |
| lahainap-v2.dtsi             | SMP_LAHAINA (439)              | 0          | 0        | 0          | 2.0 (0x20000) |
| lahainap-v2.1.dtsi           | SMP_LAHAINA (439)              | 0          | 0        | 0          | 2.1 (0x20001) |
| lahainap.dtsi                | SMP_LAHAINA_OEM_SPECIFIC (502) | 0          | 0        | 0          | 1.0 (0x10000) |
| lahainap-v2.dtsi             | SMP_LAHAINA_OEM_SPECIFIC (502) | 0          | 0        | 0          | 2.0 (0x20000) |
| lahainap-v2.1.dtsi           | SMP_LAHAINA_OEM_SPECIFIC (502) | 0          | 0        | 0          | 2.1 (0x20001) |

---

_**© 2020-2024 The Duo WOA Authors**_

_Snapdragon is a registered trademark of Qualcomm Incorporated. Microsoft, the Microsoft Corporate Logo, Windows, Surface, Surface Duo, Windows Hello, Continuum, Hyper-V, and DirectX are registered trademarks of Microsoft Corporation in the United States. Android is a registered trademark of Google LLC. Miracast is a registered trademark of the Wi-Fi Alliance. Other binaries may be copyright Qualcomm Incorporated and Microsoft Surface._

_**Limited emergency calling**_

_Running Windows on your Surface Duo is not a replacement for a proper phone operating system and does not have emergency calling capabilities._

_**Hello from Seattle (US), France, Italy.**_