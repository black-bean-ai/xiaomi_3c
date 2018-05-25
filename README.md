# mir3c router firmware

disassembled source code for the Xiaomi Router 3C

- Router Specs: <http://www.mi.com/in/mi-router-3c/specs/>
- OpenWRT Wiki Page: <https://openwrt.org/toh/xiaomi/mir3c>
- LEDE Forum Thread: <https://forum.lede-project.org/t/support-for-xiaomi-miwifi-3c/11643> (has some notes on debugging)
- Device Specs: <https://wikidevi.com/wiki/Xiaomi_MiWiFi_3C>
- Firmware URL: <http://bigota.miwifi.com/xiaoqiang/rom/r3l/miwifi_r3l_firmware_a5c81_2.9.217.bin>

# binwalk details

```

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
672           0x2A0           uImage header, header size: 64 bytes, header CRC: 0x7916E8DD, created: 2017-05-11 09:08:16, image size: 1410980 bytes, Data Address: 0x80000000, Entry Point: 0x80000000, data CRC: 0xCC31F951, OS: Linux, CPU: MIPS, image type: OS Kernel Image, compression type: lzma, image name: "MIPS OpenWrt Linux-3.10.14"
736           0x2E0           LZMA compressed data, properties: 0x6D, dictionary size: 8388608 bytes, uncompressed size: 4083808 bytes
1442464       0x1602A0        Squashfs filesystem, little endian, version 4.0, compression:xz, size: 6125436 bytes, 1832 inodes, blocksize: 262144 bytes, created: 2017-05-11 09:08:13
```

Note that the device runs OpenWRT, albeit modified.