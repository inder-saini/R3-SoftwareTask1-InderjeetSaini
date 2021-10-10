const int analog = A0; //This signal is from the arduino uno to the potentiometer, so that we can control the value on the circuit by rotating the knob
int digit_1; // This is to diplay the one's place of the number
int digit_2; // This is to display the ten's place of the number
int pot_val; // This is the value of the potentiometer,we convert the value of potentiometer which is actually from 0-1023 to 0-99 in the loop function
//BCD - 1

int a1 = 2;
int a2 = 3;
int a3 = 4;
int a4 = 5;

//BCD - 2

int b1 = 8;
int b2 = 9;
int b3 = 10;
int b4 = 11;

void setup() {
  
pinMode(2,OUTPUT);
pinMode(3,OUTPUT);
pinMode(4,OUTPUT);
pinMode(5,OUTPUT);
pinMode(8,OUTPUT);
pinMode(9,OUTPUT);
pinMode(10,OUTPUT);
pinMode(11,OUTPUT);

Serial.begin(9600);
}

void disp1(int num) {
if(num == 0){
  digitalWrite(a1,LOW);
  digitalWrite(a2,LOW);
  digitalWrite(a3,LOW);
  digitalWrite(a4,LOW);
}

 if(num == 1){
  digitalWrite(a1,HIGH);
  digitalWrite(a2,LOW);
  digitalWrite(a3,LOW);
  digitalWrite(a4,LOW);
 }

 if(num == 2){
   digitalWrite(a1,LOW);
  digitalWrite(a2,HIGH);
  digitalWrite(a3,LOW);
  digitalWrite(a4,LOW);
 }

if(num == 3){
   digitalWrite(a1,HIGH);
  digitalWrite(a2,HIGH);
  digitalWrite(a3,LOW);
  digitalWrite(a4,LOW);
}

if(num ==4){
   digitalWrite(a1,LOW);
  digitalWrite(a2,LOW);
  digitalWrite(a3,HIGH);
  digitalWrite(a4,LOW);
}

if(num == 5){
  digitalWrite(a1,HIGH);
  digitalWrite(a2,LOW);
  digitalWrite(a3,HIGH);
  digitalWrite(a4,LOW); 
}

if(num == 6){
   digitalWrite(a1,LOW);
  digitalWrite(a2,HIGH);
  digitalWrite(a3,HIGH);
  digitalWrite(a4,LOW);
}

if(num == 7){
   digitalWrite(a1,HIGH);
  digitalWrite(a2,HIGH);
  digitalWrite(a3,HIGH);
  digitalWrite(a4,LOW);
}

if(num == 8){
   digitalWrite(a1,LOW);
  digitalWrite(a2,LOW);
  digitalWrite(a3,LOW);
  digitalWrite(a4,HIGH);
}

 if(num == 9){
   digitalWrite(a1,HIGH);
  digitalWrite(a2,LOW);
  digitalWrite(a3,LOW);
  digitalWrite(a4,HIGH);
 }

}

void disp2(int num) {
if(num == 0){
  digitalWrite(b1,LOW);
  digitalWrite(b2,LOW);
  digitalWrite(b3,LOW);
  digitalWrite(b4,LOW);
}

 if(num == 1){
  digitalWrite(b1,HIGH);
  digitalWrite(b2,LOW);
  digitalWrite(b3,LOW);
  digitalWrite(b4,LOW);
 }

 if(num == 2){
   digitalWrite(b1,LOW);
  digitalWrite(b2,HIGH);
  digitalWrite(b3,LOW);
  digitalWrite(b4,LOW);
 }

if(num == 3){
   digitalWrite(b1,HIGH);
  digitalWrite(b2,HIGH);
  digitalWrite(b3,LOW);
  digitalWrite(b4,LOW);
}

if(num ==4){
   digitalWrite(b1,LOW);
  digitalWrite(b2,LOW);
  digitalWrite(b3,HIGH);
  digitalWrite(b4,LOW);
}

if(num == 5){
  digitalWrite(b1,HIGH);
  digitalWrite(b2,LOW);
  digitalWrite(b3,HIGH);
  digitalWrite(b4,LOW); 
}

if(num == 6){
   digitalWrite(b1,LOW);
  digitalWrite(b2,HIGH);
  digitalWrite(b3,HIGH);
  digitalWrite(b4,LOW);
}

if(num == 7){
   digitalWrite(b1,HIGH);
  digitalWrite(b2,HIGH);
  digitalWrite(b3,HIGH);
  digitalWrite(b4,LOW);
}

if(num == 8){
   digitalWrite(b1,LOW);
  digitalWrite(b2,LOW);
  digitalWrite(b3,LOW);
  digitalWrite(b4,HIGH);
}

 if(num == 9){
   digitalWrite(b1,HIGH);
  digitalWrite(b2,LOW);
  digitalWrite(b3,LOW);
  digitalWrite(b4,HIGH);
 }

}

void loop(){
  pot_val = map(analogRead(A0),0,1023,0,99); // Here we are converting the potentiometer value to a number between 0-99
  if(pot_val < 100)
  {
    delay(500); // This is the delay of the for about 0.5 seconds , so that the value change can occur
    pot_control(pot_val);
  }}
  void pot_control(int n){ //This function actually takes in the pot_val from function above and displays it in disp1(digit_1) which as mentioned before is one's place of a number and disp2(digit_2) which is ten's place of a number
  digit_1 = n%10; //this will store one's place
  digit_2 = n/10; //this will store ten's place

  disp1(digit_1);
  disp2(digit_2);
  
}

