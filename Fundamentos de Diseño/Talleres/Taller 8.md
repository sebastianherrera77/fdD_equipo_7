**Link de tinkercard del reto 4**

https://www.tinkercad.com/things/6qkSdUEAK80/editel?returnTo=%2Fdashboard&sharecode=k8ybANe1AcsSd422U5aHnpFf_MV9jRTf4RaS8jYrnD4

Codigos de los arduinos:

**Arduino A**

void setup() {

  Serial.begin(9600);
  
}

void loop() {

  int valor = map(analogRead(A0), 0, 1023, 0, 255);
  
  Serial.println(valor);
  
  delay(200);
  
}

**Arduino B**

const int LED = 9;

void setup() {

  Serial.begin(9600);
  
  pinMode(LED, OUTPUT);
  
}

void loop() {

  if (Serial.available()) {
  
    String linea = Serial.readStringUntil('\n');
    
    linea.trim();
    
    if (linea.length() > 0) {
    
      int valor = linea.toInt();
      
      analogWrite(LED, valor);
      
      Serial.print("Recibido: ");
      
      Serial.println(valor);
      
    }
    
  }
  
}
