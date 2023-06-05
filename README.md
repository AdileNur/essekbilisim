#include <Mouse.h>//Mouse
int xPin =A0; //Joystick x
int yPin =A1;
int buton_pin =2;
int buton durum;

int x_degeri , int y_degeri;
int xZero,yZero;
const int hassasiyet=300;


void setup()
{
pinMode(xPin,INPUT);
pinMode(yPin,INPUT);
pinMode(buton_pin,INPUT);
digitalWrite(buton_pin,HIGH);
delay(2000);
xZero = AnalogRead(xPin);
yZero = AnalogRead(yPin);


}
void loop()
{

x_degeri = AnalogRead (xPin)
xZero; //x

y_degeri = AnalogRead(yPin)
yZero;  //y

if(x_degeri != 0 || y_degeri !=0)
buton.move(x_degeri/hassasiyet,y_degeri/hassasiyet,(0);

if (digitalRead(buton_pin)&&(!buton_durum))

{
buton_durum = 1;
Mouse.press(MOUSE_LEFT);

}
else if
(digitalRead(buton_pin)&&(buton_durum))

{
buton_durum =0;

Mouse.release(MOUSE_LEFT) // sol tık kaldır;
 }
}
