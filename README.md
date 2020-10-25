# CMPE-283-Assignment-1
Binwang Luo 014632566  
Question 1.I did this assignment by myself  
Question 2. I did this assignment as below steps:  
 1. I watched the whole video "How to do the assignment 1". And I choosed to use the VMware Workstation 16 + Ubuntu 2.03. Then I installed the Vmware workstation 16 and run on Ubuntu.   
 2. Then I installed all the package I need in terminal once the VM done as below:  
   sudo apt-get install git (To install git)  
   sudo apt-get install make (To install make)  
   sudo apt-get install gcc (To install gcc)  
 3. Downloaded the files we need for this assignment in VM from Canvs (Makefile & cmpe283-1.c) and put them in the fiel named assignment1.  
 4. Open the assignment1 file in the terminal and build the file using make.   
![image](https://github.com/BinwangLuo/CMPE-283-Assignment-1/blob/main/Screenshots/make.PNG)
 5. Used ls-latr to check if the object file is created and we can see cmpe 283-1.ko. Then use commend sudo insmod ./cmpe283-1.ko & dmesg to output the initial code. 
 ![image](https://github.com/BinwangLuo/CMPE-283-Assignment-1/blob/main/Screenshots/ls-latr.PNG)  
 6. TO output the other 4 codes as request, I updated the cmpe283-1.c by looking into sdm volumn 3 section 24 for the MSRs 0x482, 0x48B, 0x483, 0x484.  
 7. After the cmpe283-1.c changing, I need to remove the moudle and insert a new moudle with sudo rmmod cmpe283-1 & sudo insmod ./cmpe283-1.ko.  
 8. Finially we can get all the output.  
 
