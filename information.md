# Forensics
First challenge in picoCTF :
![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/d85faeaf-4fb0-4e0a-a519-6cc1c89e49f6)


after we download,we have file name : cat.jpg
Step 1 : First we determine what file this is


![Screenshot from 2024-03-17 22-27-00](https://github.com/hieubmt1112004/Forensics/assets/125638408/44276acf-1eb3-471a-b4fb-0337d721cd3b)



so, this is  real image  "cat.jpg: JPEG image"
Step 2 : Let's check info 

First , We open the image file to check if there are any marks on the image by command " eog + (fileName)"

![Screenshot from 2024-03-17 22-30-34](https://github.com/hieubmt1112004/Forensics/assets/125638408/b027739a-cc8e-4d91-ae68-e3d6b3fe81ea)

In Pic , We cannot receive any information
then, we check in picture have strings ( because , flag has form strings so we check strings):

![Screenshot from 2024-03-17 22-43-27](https://github.com/hieubmt1112004/Forensics/assets/125638408/b02adc80-836d-4d8c-b7e1-15d949e94543)


this command is find string have "pico"
The flag is hidden, not given in text, which means we have to convert 1 or several more times to get the flag in the correct format
We used command "exiftool" very usedful

![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/09362991-833a-4442-8819-da96ca12035a)

we can recognize in the License case the character is encoded in 64bit
Then we decode from 64bit to text. 
This is web for you to decode : https://kt.gy/tools.html#conv/picoCTF%7Bthe_m3tadata_1s_modified%7D

![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/27cbc10e-1419-4e3b-bf42-c8449b7c20b1)

This is result : picoCTF{the_m3tadata_1s_modified}
![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/3d780f4f-7523-4696-b970-f55d7593b682)
Ye we finish first challenge! 




