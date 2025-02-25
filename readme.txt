Device Tree for OnePlus Nord 3 5G (CPH2491)

Overview

This repository contains the device tree for the OnePlus Nord 3 5G (codenamed OP5958L1). It is used for building custom ROMs and kernels for the device.

Specifications

Device: OnePlus Nord 3 5G

Model: CPH2491

Codename: OP5958L1

SoC: MediaTek Dimensity 9000 (MT6983)

CPU: Octa-core (1x3.05 GHz Cortex-X2 & 3x2.85 GHz Cortex-A710 & 4x1.80 GHz Cortex-A510)

GPU: Mali-G710 MC10

RAM: 8GB / 16GB LPDDR5

Storage: 128GB / 256GB UFS 3.1

Display: 6.74-inch, 1240 x 2772 pixels, AMOLED, 120Hz

Battery: 5000mAh, 80W Fast Charging

Camera: 50MP (OIS) + 8MP Ultra-wide + 2MP Macro | 16MP Front Camera

OS: Originally OxygenOS 13 (based on Android 13)

Building the ROM

Add the device to your build environment:

export ALLOW_MISSING_DEPENDENCIES=true
. build/envsetup.sh
lunch lineage_nord3-userdebug
make bacon -j$(nproc --all)

Replace lineage_nord3 with your ROM’s specific lunch target.

Kernel Compilation

Notes

Ensure you have the proper DTBO and vendor_boot images.

Use fastbootd to flash images when necessary.

Make sure your bootloader is unlocked before flashing.
