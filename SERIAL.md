#SERIAL on STM32CUBEIDE
>same process of creating project as "STM32 Project"
after all general steps taken keep in mind to do these as below

select the usart pin on 
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d7dcf283-ea84-4c42-9864-a85acfc94e65" />
see you had set the smae config as given in red box and keep in mind the chip must have both USART2 TX AND RX enabled



come to code file "main.c"
declare the string.h libary to use for serial
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1e968ba4-8faf-4b7b-85ca-1aef391fdfd1" />
after it check if the smae lines are their or not if not then include it
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/9f5ea8c5-1388-4c32-9e88-7763a62dd14d" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/caaf8790-ba70-4662-8da7-0e8a48ee3e2b" />
the red box is the main text declaration line


#for seeing in serial build project then after 

select the serial console
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/52550796-061c-4b20-8617-048f69edb5c4" />
a popup will come make the encoding as UTF-8
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/dbd4d3dd-eee7-403b-b64b-d056d0f334a9" />
on the red box resume as below and click on step over it runs commands line by line so at the print line you wil be able to see it in console as below

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/ce0b2bf6-ecb1-4506-b3fa-bc0c7b797fdc" />



