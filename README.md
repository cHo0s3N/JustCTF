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
## Solution:
## we are given a facebook link page! and it seems that the flag is hidden inside an image in this page! actually i was lucky! by installing the cover photo as option #1 (: which the flag was hidden inside of it! 
## let's try stegsolve! 
![solved](https://user-images.githubusercontent.com/52065067/66239992-f0a87200-e703-11e9-88e1-e53a9247e748.jpg)
###### Flag : JUST{so_you_found_me_nice_job}
# Forensics: Chopping Fl4g (82 points) >
## Description:
## Can you fix the interruptions ??
## Solution:
## we have a flag.jpg let's open it (: 
![flag](https://user-images.githubusercontent.com/52065067/66241146-13885580-e707-11e9-9d64-234d029ba90a.jpg)
## it's a really interruptions! if we try stegsolve on this we'll got nothing!
![Screenshot from 2019-10-04 17-43-14](https://user-images.githubusercontent.com/52065067/66242032-49c6d480-e709-11e9-86ae-64cbae9a0876.png)
## at the end of strings output; i got an interesting ascii art!! actually i took my time to finally fiqure what to do! 
![Screenshot from 2019-10-04 17-52-28](https://user-images.githubusercontent.com/52065067/66242571-847d3c80-e70a-11e9-97f9-ed01028b849b.png)
## just zooooooooooming out ))))):
###### Flag : JUST{Th1s_C4ll3d_Toil3t}
# Forensics: Like (94 points) >
## Description:
## I was typing then everythig gone!! Can you find my register Information plz ;(
## Solution:
## we have an image "post.jpg"!
![post](https://user-images.githubusercontent.com/52065067/66243097-f6a25100-e70b-11e9-9c9e-7e3b314b710e.jpg)
## interesting!!! the image said " i want this mockup so bad!! " and we are given a link!! 
## if you go and open this link trying to find something; it will be a waste of time! but actually i did it (:
## so now let's dive into!! the description said "Can you find my register Information plz"!!! so we are looking here for a username and a password (: or at least it must be like this! let's goooo!
![Screenshot from 2019-10-04 18-12-52](https://user-images.githubusercontent.com/52065067/66243678-1b97c380-e70e-11e9-9239-85bd05bc92f5.png)
## strings here give us nothing important! so let's try binwalk to seek any hidden files!
![Screenshot from 2019-10-04 18-13-34](https://user-images.githubusercontent.com/52065067/66243752-6ca7b780-e70e-11e9-9c73-914c5239a80f.png)
## great!!! we have a zip file and it's uncompressed as "post" here! let's cd to our extracted directory!
![Screenshot from 2019-10-04 18-15-00](https://user-images.githubusercontent.com/52065067/66244160-d6749100-e70f-11e9-9cd9-69a89f9543f5.png)
## it's a data file! let's see what's inside it!
## strings will give us too much random data lines!! so here we need our note that i mentioned it up there! that we are looking for a username and a password for regestration! so i filtered up my result!!! 
![Screenshot from 2019-10-04 18-45-05](https://user-images.githubusercontent.com/52065067/66244656-27858480-e712-11e9-8a60-baa01146b6b3.png)
## nothing here! let's try with password!
![Screenshot from 2019-10-04 18-45-46](https://user-images.githubusercontent.com/52065067/66244675-4a179d80-e712-11e9-8575-8dc689075e5f.png)
## we got here the name and it's "fl4g"!!!.... the email is base64 data just replace the url symbol %3D to "="! and decrypt it!!! 
![Screenshot from 2019-10-04 18-58-58](https://user-images.githubusercontent.com/52065067/66245014-d1194580-e713-11e9-928a-81401ec13644.png)
###### Flag : JUST{Th1s_$hould_b3_e4$y}
# Forensics: To Do List (94 points) >
## Description:
## find the passphrase to extract the flag
## solution:
## it's a jpg image! and the description here tell us what to do! we have to find the passphrase to get the flag!  
## soo! let's see if there is anything interesting inside that jpg!
![Screenshot from 2019-10-07 07-10-19](https://user-images.githubusercontent.com/52065067/66307244-9cbca980-e90c-11e9-837d-3eecff03c9cb.png)
## oops! scrolling down in strings output gave me a list of words! so let's save these words in a txt file and use it as our wordlist and see what we'll got!!
![Screenshot from 2019-10-07 07-22-35](https://user-images.githubusercontent.com/52065067/66307850-359ff480-e90e-11e9-9b76-ff8046ed1804.png)
## that was realyy faaast!! 
###### Flag : JUST{n1c3_w0rk}
# Forensics: Boring school (100 points) >
## Description:
## There is missing student can you find him in Modern School Bus
## solution:
## we are given a png image! firstly i tried stegonagraphy tools! and i got nothing! no interesting data in strings! also in the other tools which i tried! there is no any hidden files using binwalk! i checked the chunks and there size! and everything just work fine!!!! so i ended with a close road!!
![Screenshot from 2019-10-07 08-22-50](https://user-images.githubusercontent.com/52065067/66311201-9c291080-e916-11e9-9066-36fcaff17739.png)
## but who says your english skills won't benefit you! (: why would be an upper case in such ordinary word in a middle of a senetence!!!! so the missing boy i figured out that he is our flag and we have to find him in : (M)odern (S)chool (B)us ! yeah that's right in the MSB! so i opend my stegsolve trying to extract the flag!
![Screenshot from 2019-10-07 08-56-43](https://user-images.githubusercontent.com/52065067/66313558-3c813400-e91b-11e9-83b0-853078cec81a.png)
## and that's our bad boy!
###### Flag : JUST{school_is_fun}


# Forensics: Empty (100 points) >
## working on it###


# Crypto: The good rot (25 points) >
# Description: 
## WHFG{gur_nafjre_gb_yvsr_gur_havirefr_naq_rirelguvat_vf_ebg13}
## solution:
## we are given a cipher text and it seems some rotation applied here! as we notice there is #13 at the end! and #rot word up in the problem name! so let's give it a try with rot13!
![Screenshot from 2019-10-07 09-52-13](https://user-images.githubusercontent.com/52065067/66317843-f4660f80-e922-11e9-97c6-c6a7f1f10c84.png)
###### Flag : JUST{the_answer_to_life_the_universe_and_everything_is_rot13}
# Crypto: Phone (25 points) >
# Description: 
## JUST{6665553444777746665553}
## Solution:
## Keypad numbers! we have to decode this into words! i used this decoder: (http://www.aer.org/) deleting the redunduncy numbers and choosing the most sentence that make sense give us > "old is gold"
###### Flag : JUST{oldisgold}
# Crypto: Retired code (40 points) >
# Description: 
## Can you see what this code hide ??
## Solution:
## we are given two files! the first one is "code.txt" which include some binary code! the other file "hint.jfif"! i opened it to see what is says!
![hint](https://user-images.githubusercontent.com/52065067/66321104-c08de880-e928-11e9-98ac-ae525c0d8bdc.jpg)
## great! we have a sign here to lead us to which decoder we have to use! if you already have no idea what is this! you can just search for similar images on bing! at the end you'll figure that this is a BAUDOT Code! decode your binary here (https://www.boxentriq.com/code-breaking/baudot-code) and you got it!
###### Flag : JUST{BAUDOTISGOOD}
# Crypto: Call (88 points) >
# Description: 
## Can you call this number ?
## Solution:
## it's a wav file! if we play it; we'll listen to someone trying to call a number! so we have to detect these numbers! sooo by searching i got this site! (http://dialabc.com/sound/detect/) upload the file and Find our DTMF Tones! we'll got these tones: "58877778222255555563322222255" great!!! one step to get our flag! using this decoder that we use it before on "phone Q" >  (http://www.aer.org/) ... you may check how it works up here (https://www.dcode.fr/phone-keypad-cipher) 
###### Flag : JUST{CALLMECCK}
# Crypto: Mr.bean (88 points) >
# Description: 
## This my first time in London Can you help me find the flag !!
## Solution:
## we have two images!! if we open the first one "Big.png" we'll see sequence of weird symbols! 
![Big](https://user-images.githubusercontent.com/52065067/66325565-23cf4900-e930-11e9-8c07-5ea6a0d59c61.PNG)
## okaaay! what about the second image! 
![London](https://user-images.githubusercontent.com/52065067/66325896-b4a62480-e930-11e9-9705-52bd7955e950.jpg)
## Big Ben clock!!! since we have to decode that symbol given in Big image! so what the second image have to give us ?! it's just an image and does not have any important data! so after depth searching about these symbols ): i figured out what it is!! it all about your searching skills! 
## so our cipher is "Pigpen cipher" ! but what????????? the second image was our hint! big ben clock! my heart has broken here ))))): (https://www.dcode.fr/pigpen-cipher) decode your symbols and you are all set! 
###### Flag : JUST{PIGPENCIPHER}
# Crypto: Old letter (100 points) >
# Description: 
## I met foreign old man who gives me this old letter Can you read it ?
## Solution:
## we have an old letter here! contains old symbols! we have to search and search!! your key may be "old alphabet symbols" and that will give you such a huge amount of pics! 
