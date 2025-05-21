# Modified BIOS with NVME Support for SuperMicro X10SLL-F

Original BIOS file (X10SLL1.308) provided for comparison and verification.
Modified BIOS file: X10SLL1.308.NVMDXE.SMALL.bios
DXE Drivers: NVM Express v4, v5 & "Small"

Tools:
- MMTool v5.2.0.24
- UEFITool v71a (28/04/25)

Notes:
- "DXE 4" & DXE 5" are too large as-is and will write into the BIOS padding when written to the stock 308 BIOS with Aptio's Module Management Tool (MMTool). You might have better luck with CodeRush's UEFITool, but "DXE Small" works fine. DXE drivers were compiled by Ethaniel from the Win-Raid forums.

Resources:
- https://winraid.level1techs.com/t/howto-get-full-nvme-support-for-all-systems-with-an-ami-uefi-bios/30901/
- https://winraid.level1techs.com/t/howto-get-full-nvme-support-for-all-systems-with-an-ami-uefi-bios/30901/6641
- https://winraid.level1techs.com/t/guide-manual-ami-uefi-bios-modding/22633
