# JustCTF_Writeups    
# Misc: Strings (25 points) >
## Description:
## Can you read content of this file ?
## Solution:
## we are given a png image!!
![comments](https://user-images.githubusercontent.com/52065067/66232715-39efc600-e6f2-11e9-8cff-b7bdc43074e0.png)
## as we notice from the title "Strings" so >
![Screenshot from 2019-10-04 15-12-33](https://user-images.githubusercontent.com/52065067/66233711-aa97e200-e6f4-11e9-8f94-5b2229463fbe.png)
###### Flag : JUST{y3s_y0u_c4n}
# Misc: RegEX (40 points) >
## Description: 
## flag is one of this!! Can you find the only upper case flag??
## Solution:
## we are given a flags.txt and we need to find the only upper case flag!!!
## if you count the number of lines in flags.txt it will be 1468 sooooo!
![Screenshot from 2019-10-04 15-30-23](https://user-images.githubusercontent.com/52065067/66234677-f6e42180-e6f6-11e9-992d-3914f015d03c.png)
###### Flag : JUST{BAD_R3GEX}
# Misc: Catch me (52 points) >
## Description:
## catch me if you can ?
## Solution:
## we have here a zip file! If you unzip this we will got many hidden files!
![Screenshot from 2019-10-04 15-43-37](https://user-images.githubusercontent.com/52065067/66235648-3f9cda00-e6f9-11e9-89b7-f25e0ca92b46.png)
## useless!!! let's try something else.. since we got hidden files we can try binwalk on the zip file!! 
![Screenshot from 2019-10-04 15-45-43](https://user-images.githubusercontent.com/52065067/66235857-bc2fb880-e6f9-11e9-8407-8d4561cb6c82.png)
## let's move to the directory and see what we got!
![Screenshot from 2019-10-04 15-46-02](https://user-images.githubusercontent.com/52065067/66235958-fd27cd00-e6f9-11e9-8251-757bdcbcf955.png)
## and yeah we got the flag! easy!
###### Flag : JUST{Y0u_c0ught_m3}
# Misc: .docx (64 points) >
## Description:
## i can't open this docx file can you help me with that :)
## solution:
## so we have a docx file,, double tab and we got this!
![Screenshot from 2019-10-04 16-06-09](https://user-images.githubusercontent.com/52065067/66236712-e4201b80-e6fb-11e9-8c73-971a4c021aa0.png)
## ohh it's protected with a password! let's help him open this up!
![Screenshot from 2019-10-04 16-14-56](https://user-images.githubusercontent.com/52065067/66237112-f2bb0280-e6fc-11e9-8f74-f386cb77bc37.png)
## CDFV2 (Composite Document File V2) Encrypted!! since it's a word office document we can use john to decrypt it!
![Screenshot from 2019-10-04 16-27-02](https://user-images.githubusercontent.com/52065067/66237903-e89a0380-e6fe-11e9-99e8-4cccd0c10af5.png)
## nice! we got the hash value! let's crack it!!!!!!!!
![Screenshot from 2019-10-04 16-32-39](https://user-images.githubusercontent.com/52065067/66238067-60682e00-e6ff-11e9-853f-49792f9f0fa4.png)
## oops! the password was password!!!! tricky one? 
![Screenshot from 2019-10-04 16-37-01](https://user-images.githubusercontent.com/52065067/66238526-79251380-e700-11e9-86b5-4827a3133e04.png)
###### Flag : JUST{m1cr0$oft_w0rd}
# Forensics: f4c3book (73 points) >
## Description: 
## find the flag in this page (https://www.facebook.com/HackerSpace_JUST-107702673912712)
## we are given a facebook link page! and it seems that the flag is hidden inside an image in this page! actually i was lucky! by installing the cover photo as option #1 (: which the flag was hidden inside of it! 
## let's try stegsolve! 





