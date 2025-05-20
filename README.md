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
python LN882H_Flash_Dumper.py COM3 download flash 2000000 0x0 OpenLN882H_1.17.427.bin
```
