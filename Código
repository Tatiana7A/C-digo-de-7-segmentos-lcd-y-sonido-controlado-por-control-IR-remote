#include <LiquidCrystal.h>
#include <IRremote.h>

int IRpin = 9;
LiquidCrystal lcd(32, 31, 25, 24, 23, 22);

void setup() {

  Serial.begin(9600);
  IrReceiver.begin(IRpin);
  //pin de conexión de sonido
  pinMode (36, OUTPUT);

//pines de conexión 7 segmentos
  pinMode (3, OUTPUT);      //b
  pinMode (4, OUTPUT);      //c
  pinMode (5, OUTPUT);
  pinMode (6, OUTPUT);
  pinMode (7, OUTPUT);
  pinMode (8, OUTPUT);
  pinMode (2, OUTPUT);
  pinMode(36,OUTPUT);

//Mensaje de presentación en LCD  
  lcd.begin(16,2);
  lcd.setCursor(3,0);
  lcd.print("Bienvenidos");
  delay(2000);
  lcd.clear();

  lcd.setCursor(5,0);
  lcd.print("Tatiana");
  lcd.setCursor(5,1);
  lcd.print("Ochoa");
  delay(2000);
  lcd.clear();

    lcd.setCursor(5,0);
  lcd.print("Control");
  lcd.setCursor (4,1);
  lcd.print ("infrarojo");
  delay (2000);
  lcd.clear();
}

void loop() {

  while (IrReceiver.decode() == 0) {
  }

  int signalRf = IrReceiver.decodedIRData.command;
  Serial.println(signalRf);
  delay(500);
  IrReceiver.resume();
  if(signalRf==22){
     digitalWrite(36,HIGH);
    delay(300);
    digitalWrite (2,HIGH);
    digitalWrite (3,HIGH);
    digitalWrite (4,HIGH);
    digitalWrite (5,HIGH);
    digitalWrite (6,HIGH);
    digitalWrite (7,HIGH);
    digitalWrite (8,LOW );
    lcd.clear();
    lcd.setCursor(1,0);
    lcd.print("Numero 0");
    lcd.setCursor (1,1);
    lcd.print("presionado");
    delay (300);
  }
  if(signalRf==12){
    digitalWrite(36,HIGH);
    delay(300);
    digitalWrite(36,LOW);
    digitalWrite (3,HIGH);
    digitalWrite (4,HIGH);
    digitalWrite (2,LOW);
    digitalWrite (5,LOW);
    digitalWrite (6,LOW);
    digitalWrite (7,LOW);
    digitalWrite (8, LOW);
    lcd.clear();
    lcd.setCursor(1,0);
    lcd.print("Numero 1");
    lcd.setCursor (1,1);
    lcd.print("presionado");
    delay (300);
  }
  if(signalRf==24){
     digitalWrite(36,HIGH);
    delay(300);
    digitalWrite (2,HIGH);
    digitalWrite (3,HIGH);
    digitalWrite (4,LOW);
    digitalWrite (5,HIGH);
    digitalWrite (6,HIGH);
    digitalWrite (7,LOW);
    digitalWrite (8,HIGH );
    lcd.clear();
    lcd.setCursor(1,0);
    lcd.print("Numero 2");
    lcd.setCursor (1,1);
    lcd.print("presionado");
    delay (300);
  }
  if(signalRf==94){
     digitalWrite(36,HIGH);
    delay(300);
    digitalWrite (2,HIGH);
    digitalWrite (3,HIGH);
    digitalWrite (4, HIGH);
    digitalWrite (5,HIGH);
    digitalWrite (6,LOW);
    digitalWrite (7,LOW);
    digitalWrite (8,HIGH );
    lcd.clear();
    lcd.setCursor(1,0);
    lcd.print("Numero 3");
    lcd.setCursor (1,1);
    lcd.print("presionado");
    delay (300);
  }
  if(signalRf==8){
     digitalWrite(36,HIGH);
    delay(300);
    digitalWrite (2,LOW);
    digitalWrite (3,HIGH);
    digitalWrite (4,HIGH);
    digitalWrite (5,LOW);
    digitalWrite (6,LOW);
    digitalWrite (7,HIGH);
    digitalWrite (8,HIGH );
    lcd.clear();
    lcd.setCursor(1,0);
    lcd.print("Numero 4");
    lcd.setCursor (1,1);
    lcd.print("presionado");
    delay (300);
  }
  if(signalRf==28){
     digitalWrite(36,HIGH);
    delay(300);
    digitalWrite (2,HIGH);
    digitalWrite (3,LOW);
    digitalWrite (4,HIGH);
    digitalWrite (5,HIGH);
    digitalWrite (6,LOW);
    digitalWrite (7,HIGH);
    digitalWrite (8,HIGH );
    lcd.clear();
    lcd.setCursor(1,0);
    lcd.print("Numero 5");
    lcd.setCursor (1,1);
    lcd.print("presionado");
    delay (300);
  }
  if(signalRf==90){
     digitalWrite(36,HIGH);
    delay(300);
    digitalWrite (2,HIGH);
    digitalWrite (3,LOW);
    digitalWrite (4,HIGH);
    digitalWrite (5,HIGH);
    digitalWrite (6,HIGH);
    digitalWrite (7,HIGH);
    digitalWrite (8,HIGH );
    lcd.clear();
    lcd.setCursor(1,0);
    lcd.print("Numero 6");
    lcd.setCursor (1,1);
    lcd.print("presionado");
    delay (300);
  }
  if(signalRf==66){
     digitalWrite(36,HIGH);
    delay(300);
    digitalWrite (2,HIGH);
    digitalWrite (3,HIGH);
    digitalWrite (4,HIGH);
    digitalWrite (5,LOW);
    digitalWrite (6,LOW);
    digitalWrite (7,LOW);
    digitalWrite (8,LOW);
    lcd.clear();
    lcd.setCursor(1,0);
    lcd.print("Numero 7");
    lcd.setCursor (1,1);
    lcd.print("presionado");
    delay (300);
  }
  if(signalRf==82){
     digitalWrite(36,HIGH);
    delay(300);
    digitalWrite (2,HIGH);
    digitalWrite (3,HIGH);
    digitalWrite (4,HIGH);
    digitalWrite (5,HIGH);
    digitalWrite (6,HIGH);
    digitalWrite (7,HIGH);
    digitalWrite (8,HIGH );
    lcd.clear();
    lcd.setCursor(1,0);
    lcd.print("Numero 8");
    lcd.setCursor (1,1);
    lcd.print("presionado");
    delay (300);
  }
  if(signalRf==74){
     digitalWrite(36,HIGH);
    delay(300);
    digitalWrite (2,HIGH);
    digitalWrite (3,HIGH);
    digitalWrite (4,HIGH);
    digitalWrite (5,HIGH);
    digitalWrite (6,LOW);
    digitalWrite (7,HIGH);
    digitalWrite (8,HIGH);
    lcd.clear();
    lcd.setCursor(1,0);
    lcd.print("Numero 9");
    lcd.setCursor (1,1);
    lcd.print("presionado");
    delay (300);
  }
 if(signalRf==69){
   digitalWrite(36,HIGH);
    delay(300);
    digitalWrite (2,LOW);
    digitalWrite (3,LOW);
    digitalWrite (4,LOW);
    digitalWrite (5,LOW);
    digitalWrite (6,LOW);
    digitalWrite (7,LOW);
    digitalWrite (8,LOW );
    lcd.clear();
    lcd.setCursor(1,0);
    lcd.print("Apagado");
    delay (300);
  }
}
