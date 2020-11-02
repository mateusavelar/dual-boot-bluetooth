First, Pair in Linux, then pair in Windows... 
___
then run:

./pstools/psexec.exe -s -i regedit /e C:\temp\dual-boot-bluetooth-pair-master\BTKeys.reg HKEY_LOCAL_MACHINE\SYSTEM\ControlSet001\Services\BTHPORT\Parameters\Keys


python.exe .\clean_reg_file.py BTKeys.reg keys.reg


python.exe .\bluetooth_fix.py --reg_path .\keys.reg > info.txt



-------
get back on linux and update the info file from the previus paring.
restart bluethooth service.
