# Audio Salad | ஆடியோ சாலட்

## Forensics | தடயவியல்

### Source File : Audiosalad.wav
**Question : My friend sent me this message via audio, but I dropped my salad on my computer before I could listen to it. Help!!!**

>First i had think , There is Audio Steganography. By doing the below things, I had got the message from Audio.

<ins>Step - 1<ins> : 
- Download the Source File and [Sonic-Visualiser](https://www.sonicvisualiser.org/)
- Install sonic-visualiser

![image](https://user-images.githubusercontent.com/76644058/199799937-ccca8e4e-7345-4915-a606-28d2b958c0b5.png)


<ins>Step - 2<ins> : 
- Open the AudioFile in Sonic-visualiser
  
![image](https://user-images.githubusercontent.com/76644058/199800489-5e926e25-7961-4e4d-b6a5-9c7e55777536.png)

  
<ins>step - 3<ins> :
- Then add steg layer , which is persent in the layeropion
  ![image](https://user-images.githubusercontent.com/76644058/199800879-7c1880a6-f158-4484-be47-6824fb4d67c5.png)  
- Now got some meaning less number
- The number is : 49 52 51 48 54 7b 31 33 6f ...

<ins>step - 4<ins> :
- I guess this is Hexadecimal Number.Use [Cipher chef](https://gchq.github.io/CyberChef/)
  ![image](https://user-images.githubusercontent.com/76644058/199802434-7c00661a-d3c5-4a39-9f05-07dbe62c7045.png)
- So i can try to change Hexadecimal Number to Characters.
- Happy to see Message [Flag : IRQHT{xxxxxxxxxxxxxxx}] But Not correct
- Then Apply ceaser cipher to decrypt [ROT12](https://rot13.com/)
  
  ![image](https://user-images.githubusercontent.com/76644058/199802915-f8fcd5a1-f91a-449f-a128-e21962ac5991.png)
  
- Final Flag : [UDCTF{13s....}]
  
  
# <p align="center">நன்றி :pray: வணக்கம்</p>
