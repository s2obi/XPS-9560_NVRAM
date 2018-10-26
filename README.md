# XPS 15 9560 NVRAM EDIT

### Example IFR dump for intel SST option
```
0x371A8   Setting: Intel(R) Speed Shift Technology, Variable: 0x4BC {05 91 B3 01 B4 01 E3 01 01 00 BC 04 10 10 00 01 00}
0x371B9     Option: Disabled, Value: 0x0 {09 07 04 00 30 00 00}
0x371C0     Option: Enabled, Value: 0x1 {09 07 03 00 00 00 01}
0x371C7   End of Options {29 02}
```

### If you want to enable SST, boot for UEFI Shell first and write the following and press enter
###### __*warning! this may brick your machine, use at your own risk*__
```
setup_var 0x4BC 0x1
```
