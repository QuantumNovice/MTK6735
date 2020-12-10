# MTK6735/53

* Stuff related to mt6735 specifically

# Scatter 
## General Info 
```
- general: MTK_PLATFORM_CFG
  info:
    - config_version: V1.1.2
      platform: MT6753
      project: gionee6753_65u_m0
      storage: EMMC
      boot_channel: MSDC_0
      block_size: 0x20000
```
## Layout
```
- partition_index: SYS0
  partition_name: preloader
  file_name: preloader_gionee6753_65u_m0.bin
  is_download: true
  type: SV5_BL_BIN
  linear_start_addr: 0x0
  physical_start_addr: 0x0
  partition_size: 0x400000
  region: EMMC_BOOT_1
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: BOOTLOADERS
  reserve: 0x00

- partition_index: SYS1
  partition_name: pgpt
  file_name: NONE
  is_download: false
  type: NORMAL_ROM
  linear_start_addr: 0x0
  physical_start_addr: 0x0
  partition_size: 0x80000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: INVISIBLE
  reserve: 0x00

- partition_index: SYS2
  partition_name: proinfo
  file_name: NONE
  is_download: false
  type: NORMAL_ROM
  linear_start_addr: 0x80000
  physical_start_addr: 0x80000
  partition_size: 0x300000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: PROTECTED
  reserve: 0x00

- partition_index: SYS3
  partition_name: nvram
  file_name: NONE
  is_download: false
  type: NORMAL_ROM
  linear_start_addr: 0x380000
  physical_start_addr: 0x380000
  partition_size: 0x500000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: BINREGION
  reserve: 0x00

- partition_index: SYS4
  partition_name: protect1
  file_name: NONE
  is_download: false
  type: NORMAL_ROM
  linear_start_addr: 0x880000
  physical_start_addr: 0x880000
  partition_size: 0xA00000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: PROTECTED
  reserve: 0x00

- partition_index: SYS5
  partition_name: protect2
  file_name: NONE
  is_download: false
  type: NORMAL_ROM
  linear_start_addr: 0x1280000
  physical_start_addr: 0x1280000
  partition_size: 0xA00000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: PROTECTED
  reserve: 0x00

- partition_index: SYS6
  partition_name: lk
  file_name: lk.bin
  is_download: true
  type: NORMAL_ROM
  linear_start_addr: 0x1C80000
  physical_start_addr: 0x1C80000
  partition_size: 0x80000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: UPDATE
  reserve: 0x00

- partition_index: SYS7
  partition_name: para
  file_name: NONE
  is_download: false
  type: NORMAL_ROM
  linear_start_addr: 0x1D00000
  physical_start_addr: 0x1D00000
  partition_size: 0x80000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: INVISIBLE
  reserve: 0x00

- partition_index: SYS8
  partition_name: boot
  file_name: boot.img
  is_download: true
  type: NORMAL_ROM
  linear_start_addr: 0x1D80000
  physical_start_addr: 0x1D80000
  partition_size: 0x1000000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: UPDATE
  reserve: 0x00

- partition_index: SYS9
  partition_name: recovery
  file_name: recovery.img
  is_download: true
  type: NORMAL_ROM
  linear_start_addr: 0x2D80000
  physical_start_addr: 0x2D80000
  partition_size: 0x1000000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: UPDATE
  reserve: 0x00

- partition_index: SYS10
  partition_name: logo
  file_name: logo.bin
  is_download: true
  type: NORMAL_ROM
  linear_start_addr: 0x3D80000
  physical_start_addr: 0x3D80000
  partition_size: 0x800000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: UPDATE
  reserve: 0x00

- partition_index: SYS11
  partition_name: expdb
  file_name: NONE
  is_download: false
  type: NORMAL_ROM
  linear_start_addr: 0x4580000
  physical_start_addr: 0x4580000
  partition_size: 0xA00000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: INVISIBLE
  reserve: 0x00

- partition_index: SYS12
  partition_name: seccfg
  file_name: NONE
  is_download: false
  type: NORMAL_ROM
  linear_start_addr: 0x4F80000
  physical_start_addr: 0x4F80000
  partition_size: 0x80000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: INVISIBLE
  reserve: 0x00

- partition_index: SYS13
  partition_name: oemkeystore
  file_name: NONE
  is_download: false
  type: NORMAL_ROM
  linear_start_addr: 0x5000000
  physical_start_addr: 0x5000000
  partition_size: 0x200000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: INVISIBLE
  reserve: 0x00

- partition_index: SYS14
  partition_name: secro
  file_name: secro.img
  is_download: true
  type: NORMAL_ROM
  linear_start_addr: 0x5200000
  physical_start_addr: 0x5200000
  partition_size: 0x600000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: UPDATE
  reserve: 0x00

- partition_index: SYS15
  partition_name: keystore
  file_name: NONE
  is_download: false
  type: NORMAL_ROM
  linear_start_addr: 0x5800000
  physical_start_addr: 0x5800000
  partition_size: 0x800000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: INVISIBLE
  reserve: 0x00

- partition_index: SYS16
  partition_name: tee1
  file_name: tz1.img
  is_download: true
  type: NORMAL_ROM
  linear_start_addr: 0x6000000
  physical_start_addr: 0x6000000
  partition_size: 0x500000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: UPDATE
  reserve: 0x00

- partition_index: SYS17
  partition_name: tee2
  file_name: tz2.img
  is_download: true
  type: NORMAL_ROM
  linear_start_addr: 0x6500000
  physical_start_addr: 0x6500000
  partition_size: 0x500000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: UPDATE
  reserve: 0x00

- partition_index: SYS18
  partition_name: frp
  file_name: NONE
  is_download: false
  type: NORMAL_ROM
  linear_start_addr: 0x6A00000
  physical_start_addr: 0x6A00000
  partition_size: 0x100000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: PROTECTED
  reserve: 0x00

- partition_index: SYS19
  partition_name: nvdata
  file_name: NONE
  is_download: false
  type: NORMAL_ROM
  linear_start_addr: 0x6B00000
  physical_start_addr: 0x6B00000
  partition_size: 0x2000000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: INVISIBLE
  reserve: 0x00

- partition_index: SYS20
  partition_name: metadata
  file_name: NONE
  is_download: false
  type: NORMAL_ROM
  linear_start_addr: 0x8B00000
  physical_start_addr: 0x8B00000
  partition_size: 0x2500000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: INVISIBLE
  reserve: 0x00

- partition_index: SYS21
  partition_name: system
  file_name: system.img
  is_download: true
  type: EXT4_IMG
  linear_start_addr: 0xB000000
  physical_start_addr: 0xB000000
  partition_size: 0xF0000000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: UPDATE
  reserve: 0x00

- partition_index: SYS22
  partition_name: cache
  file_name: cache.img
  is_download: true
  type: EXT4_IMG
  linear_start_addr: 0xFB000000
  physical_start_addr: 0xFB000000
  partition_size: 0x19000000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: UPDATE
  reserve: 0x00

- partition_index: SYS23
  partition_name: userdata
  file_name: userdata.img
  is_download: true
  type: EXT4_IMG
  linear_start_addr: 0x114000000
  physical_start_addr: 0x114000000
  partition_size: 0x632B80000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: true
  is_reserved: false
  operation_type: UPDATE
  reserve: 0x00

- partition_index: SYS24
  partition_name: flashinfo
  file_name: NONE
  is_download: false
  type: NORMAL_ROM
  linear_start_addr: 0xFFFF0084
  physical_start_addr: 0xFFFF0084
  partition_size: 0x1000000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: false
  is_reserved: true
  operation_type: RESERVED
  reserve: 0x00

- partition_index: SYS25
  partition_name: sgpt
  file_name: NONE
  is_download: false
  type: NORMAL_ROM
  linear_start_addr: 0xFFFF0004
  physical_start_addr: 0xFFFF0004
  partition_size: 0x80000
  region: EMMC_USER
  storage: HW_STORAGE_EMMC
  boundary_check: false
  is_reserved: true
  operation_type: RESERVED
  reserve: 0x00
```
