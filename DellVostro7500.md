# Dell Vostro 7500

## 安装 Ubuntu 注意事项

* 确保 BIOS 设为 UEFI， 禁用 Legacy Option ROMS 和 Secure Boot.

## 分区情况

| 分区 | 大小 | 挂载点 |
|    :---:    |    ---:   |    ---    |
| nvme0n1p1 |   100M | /boot/efi |
| nvme0n1p2 |    50G | /         |
| nvme0n1p3 | 350.9G | /home     |
| nvme0n1p4 |    60G | /opt      |
| nvme0n1p5 |    16G | [SWAP]    |
