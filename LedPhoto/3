#define sensor_pin A0
#define led_pin 3

void setup() {
  Serial.begin(9600);
  pinMode(led_pin, OUTPUT);
}

void loop() {
  int val = analogRead(sensor_pin);
  if (val<40){//менять val в зависимости от сенсора
  int ledPower = map(val, 0, 70, 255, 0);//значения map настроить от val
  analogWrite(led_pin, ledPower);
  Serial.println(ledPower);}
  digitalWrite(led_pin, LOW);    
  
}
