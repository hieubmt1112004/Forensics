Today we will solve the challenge is : MacroHard WeakEdge



![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/9753cea4-9ad4-4f69-943d-73fab4df3391)



This is we challenge! 

file ending is .pptm is file powerpoint! 
On request it looks like 1 previous challenge did!
First we check file 

![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/a1c1ddea-877e-407f-bf2e-fa263140cf61)


File :Microsoft PowerPoint 2007+
We open file 



![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/c61a52ad-c654-45e4-968b-302fb217ae5c)



To see the contents behind this file we must extract to see all the files inside




![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/a87acf6c-93c6-4147-ae92-efe62ccb3c19)




Then we have a file '_Forensics is fun.pptm.extracted' . We check each file one by one

After quite a long time I checked each file one by one. 

I opened a 'hidden' file with the path "Forensics is fun.pptm.extracted/ppt/slideMasters"




![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/ef78436f-a4b2-46c7-a8d1-0b8d754a66c4)





Let's check file "hidden" :


![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/d288b538-59d6-49fe-a9d0-7866f7dcaf53)




"Z m x h Z z o g c G l j b 0 N U R n t E M W R f d V 9 r b j B 3 X 3 B w d H N f c l 9 6 M X A 1 f Q"


seem like base64. let's decode 



![image](https://github.com/hieubmt1112004/Forensics/assets/125638408/080ffd74-d82b-4dec-8ec1-e03f51d18089)



This is flag: picoCTF{D1d_u_kn0w_ppts_r_z1p5}











