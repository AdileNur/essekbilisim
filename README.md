#include <Mouse.h>

int xPin =A0;
int yPin =A1;
int solButon =5;
int sagButon =4;
int x_degeri,y_degeri;
int IlkDeger,yIlkDeger;
int hassasiyet =300;


void setup()
{
  pinMode(xPin,INPUT);
  pinMode(yPin,INPUT);
  pinMode(solButon,INPUT);
  pinMode(sagButon,INPUT);
  int xIlkDeger = analogRead (xPin);
  int yIlkDeger = analogRead (yPin);
  
  }
  
  void loop()
 x_degeri = analogRead(XPin) - xIlkDeger;
 y_degeri = analogRead(YPin) - yIlkDeger;
 
 if(x_degeri ! = 0 || y_degeri ! = 0)
  Mouse.move(x_degeri / hassaysiyet , y_degeri / hassasiyet, 0);
  
  if(digitalRead(solButon) == 1) Mouse.press(MOUSE_LEFT);
  else Mouse.release(MOUSE_ LEFT);
  
  if(digitalRead(sagButon) == 1)Mouse.press(MOUSE_RIGHT);
  else Mouse.release(Mouse_RIGHT);
  }
  
  
