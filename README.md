
// C++ code for Tempsensor
int tempsensor;
void setup()
{
 pinMode(A2,INPUT);
pinMode(12,OUTPUT);
 pinMode(13,OUTPUT);
 
}
void loop()
{
 tempsensor=analogRead(A2);
 if(tempsensor>=200)
 {
 digitalWrite(13,HIGH);
 tone(12,500,500);
 }
 digitalWrite(13,LOW);
}
-------------------------------------------
// C++ code for obstacle detection
int pirsensor;
void setup()
{
 pinMode(2,INPUT);
pinMode(12,OUTPUT);
 pinMode(13,OUTPUT);
 
}
void loop()
{
 pirsensor=digitalRead(2);
 if(pirsensor==HIGH)
 {
 digitalWrite(13,HIGH);
 tone(12,1000,1000);
 }
 digitalWrite(13,LOW);
}
--------------------------------------------------
cd Desktop/
hello.cpp
g++ hello.cpp
./a.out
-----------------
javac FIFO.java
java FIFO
------------
