
#define pinSensorA A0
#define rele 7

void setup() {
  pinMode (pinSensorA, INPUT);
  pinMode (rele, OUTPUT);

  digitalWrite (rele, LOW);
}

void loop() {
  if (analogRead(pinSensorA)>700){
    digitalWrite (rele, HIGH);   
  } else {
    digitalWrite (rele, LOW);
  }
  
}
