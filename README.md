# R3-SoftwareTask1-InderjeetSaini

This is the first task from R3 Robotics team for Software Training.

I have done the following task by doing the following steps:

At first, I studied about the various parts that have been mentioned to use and what their functions are
Then, I tried to create the circuit in Tinkercad as I did not have the actuall breadboard and components
As, I had experience working with a seven seg,ent display first in the course 328, I knew some concepts about the seven seg,ent display. Here I have used Common Cathode Seven segment display which grounds its pins 3 and 8.
Also, I had studied about the decoder in the same course. Here, I was confused about how to write a code in arduino as I did not have much experience with it.
However, it hit my mind that since we are connecting only potentiometer (analog signal). to arduino and the digital signals to the two decoders(CD4511), I just need to code in arduino taking them into consideration. As, the decoder will then in turn will work with seven segment display.
I also had to learn how to connect the decoder as there were three pins which I was not sure about namely: Lamp Test,Blanking and Latch Enable. I found a online source in which I learned that usually we keep Lamp Test and Blanking on High, and Latch Enable on Low to get High output.
After, making the whole circit, All that was left was for to write the code in arduino which was not that tricky except for the potentimeter part. At first, I realized I had made a 2- digit counter but then had to make some changes in the loop function which lead me to gain the control from the potentiometer.


The link to my circuit is here:
https://www.tinkercad.com/things/l7h8ITL3gh8
