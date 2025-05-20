# LN822H_dump_tool

Tool to help backup fw and flash https://github.com/openshwprojects/OpenBK7231T_App for LN822N chips.

FW flasher and its Python wrapper(initial version) taken from https://www.elektroda.com/rtvforum/topic4028087.html

Example backup (replace COM3 with your device):

```bash
python LN882H_Flash_Dumper.py COM3 backup 0x0200000
```

Another example backup:

```bash
python LN882H_Flash_Dumper.py COM3 flashdump
```

Example flash:

```bash
./LN882H_CMD_Tool.exe COM3 download flash 2000000 0x0 OpenLN882H_1.18.102.bin
```

The script was updated to be able to handle frequent read errors that I encountered, and actually show progress since the dump takes 15~+ minutes:

[![Backup screenshot](docs/backup.png?raw=true)](docs/backup.png?raw=true)
