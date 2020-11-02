Pair first in Linux, then pair in Windows... then

1* 
./pstools/psexec.exe -s -i regedit /e C:\temp\dual-boot-bluetooth-pair-master\BTKeys.reg HKEY_LOCAL_MACHINE\SYSTEM\ControlSet001\Services\BTHPORT\Parameters\Keys
2*
python.exe .\clean_reg_file.py BTKeys.reg keys.reg
3*
python.exe .\bluetooth_fix.py --reg_path .\keys.reg > info.txt



get back on linux and update the info file from the previus paring.
restart bluethooth service.