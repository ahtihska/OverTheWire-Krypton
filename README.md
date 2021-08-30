# OverTheWire Natas  
<br>

 Solution for Natas levels on [OverTheWire](https://overthewire.org/wargames/krypton/)
  ## Contents
* [Level 0 - Level 1](#level-0---level-1)
* [Level 1 - Level 2](#level-1---level-2)
## Level 0 - Level 1
The password is encoded using Base64.
```
string: S1JZUFRPTklTR1JFQVQ=
decoded string: KRYPTONISGREAT
```
Log in to krypton.labs.overthewire.org with username krypton1 using SSH on port 2231
``` 
ssh krypton1@krypton.labs.overthewire.org -p 2231
Password: KRYPTONISGREAT
```
## Level 1 - Level 2
The password for level 2 is stored in the file krypton2.
```
pwd
cd /krypton/krypton1
cat krypton2
```
The password is encoded with simple rotation
```
cat krypton2 | tr "[a-zA-Z]" "[n-za-mN-ZA-M]
string:YRIRY GJB CNFFJBEQ EBGGRA
decoded string: LEVEL TWO PASSWORD ROTTEN
   
