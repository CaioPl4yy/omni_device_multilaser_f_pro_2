# Android device tree for Multilaser F Pro 2 (Multilaser_F_Pro_2)

Unisoc SC9832E (sp9832e_1h10_go), Android 11, 32-bit userspace, Virtual A/B, recovery-as-boot.

Generated with SebaUbuntu's twrpdtgen, then checked against the stock boot.img
and partition XML from firmware V6_20220223.

Changes over the generated tree:
- Correct super partition size (2500 MiB) and group size
- Removed BOARD_RECOVERYIMAGE_PARTITION_SIZE (there is no recovery partition)
- FBE/metadata decryption flags copied from the stock fstab (untested)
- stock_kernel.config: config extracted from the stock kernel (4.14.193), for reference

Status: UNTESTED on hardware.
