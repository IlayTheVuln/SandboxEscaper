# SandboxEscaper
A sandbox ecapare i wrote in cs!
2 files:
ststic class that holds data of othet antimalware programs(AntiMalwareDataBase)
static class that uses this database and preform the checks(SandBoxEscaper)
the sandbox escaper is a static class that contains a database of many known AV, EDR, WinDefender resources.
the edrs,avs it is checking are:
Eset
BitDefender
VGA
Norton
Sophos
TrendMicro
Avast
McAffee

!!feel free to add more rendors by sending me an email:ilaysam00@gmail.com
and ill add them in the "AntiMalwareDataBase"!!


it is prefoeming theses checks in order to test for suspicious runtime environment:

1. vm resources=>checks for known names of files that are used for creating a vm to test the malware
2.processes and services=>checks for known names of 
3.BiosId=>vm's usually uses a new massive and obfussicated biosid so the sandbox escaper checks taht
4.Manufactorer=>check weathet the manufactorer of the "pc" is identified with known sandbox conventions

