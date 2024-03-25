Challenge : TrivialFlagTransferProtocol
Points : 90 

today we will solve challenge .PCAP, for .pcap articles, we need the program to open. Wireshark, for example.


![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/84c4e1f9-ded3-469a-abc3-249ae54b01b2)



After downloading the pcap file, we proceed to open the file with the Wireshark application


![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/6ccbf830-c27b-47b6-836c-f0700cff0b84)


In the first in protocol TFTP , we see file instructions.txt,this is the first questionable point, so we view all file in TFTP

![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/5a17642c-bd18-4bfd-afef-4bbd4a1ea0bd)



![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/ab0a1eab-723b-40ae-9c2e-596b5da4816b)



wao this is anything we need , we save all file.
After save file we start to check to find the flag

![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/d3c18929-567b-4602-93f9-c43934c8db1b)

start to open the file txt 

![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/b0eda0c4-de9e-43e1-9e21-b46ec0ce8d9f)


we decode by https://www.dcode.fr 
![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/bb6db5db-3ef2-4d70-8077-f9d32afc4ab1)



It is ROT-13 Cipher, after decode "instructions.txt" have infomations : " TFTP DOESNT ENCRYP TOUR TRAFFIC SOWE MUST DISGUISEOUR FLAGT RANSFER.FIGURE OUT AWAY TO HIDE THE FLAG AND I WILL CHECK BACK FOR THE PLAN"

And decode "plan.txt" : "I USED THE PROGRAM AND HIDIT WITH-DUEDILIGENCE.CHECK OUT THE PHOTOS"

Let's extracted to read file program.deb by dpkg-deb -xv (file.deb) + (newfilename)


![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/d1c1f51e-50a2-4b20-bec2-85d0fa72e3e8)



to open file after extracted :

![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/67cee4a5-fbc4-4990-a700-49d00b9f8176)


we have a keyword " steghide ". What is steghide ? 



![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/6703cfac-33a4-4bab-ba88-7ef5234f5ad1)


To check if information is hidden in the file, use the command " steghide info + (file)"


first is pic1 : 


![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/4311ba50-a627-45f4-a48f-4c560b8e84e5)


it's locked, we need password, we can find in file txt. There is only 1 most suspicious thing in all that keyword is"DUEDILIGENCE". we can check 3 photos 



![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/80ff81c9-35fc-4680-8a7a-81a63641be8b)


Data in picture3. let's extract pic3 to received flag.txt


![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/a30c197d-fa10-4172-82fe-5756627aa83b)


Flag  :  picoCTF{h1dd3n_1n_pLa1n_51GHT_18375919} 



































