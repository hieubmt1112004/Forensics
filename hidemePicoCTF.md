Today we will solve challenge 100 points. 



![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/64397195-4129-4f48-bc8b-ecc97329c754)

First we check file type. 


![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/79bbcc12-24b9-41ab-8f57-26685934b062)


Then we find flag(strings) in image 



![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/a5125544-6de0-4ca1-8ecb-b5a172561522)


Don't have anything


Next ,We analyze images using ExifTool



![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/038299d4-e6f9-4360-a29b-67e9dd8ba5b9)



We focus on Warning : It means that there is still data behind the photo
We need to compress the file to see all the hidden files of the image



![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/951d7833-6788-46ef-90e9-15e186140e16)



This is file flag after extracted.


Let's check file flag


![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/98f87002-d2e8-4c4a-b6fe-a9f7c40ee6e6)


This is flag : picoCTF{Hiddinng_An_imag3_within_@n_ima9e_82101824}

Take 100 points very easy! Congratulations









