# Trash-Repo


Exp 2 - LED bar
https://www.tinkercad.com/things/1gTyVIxaHSB-experiment-2-led-bar/editel?returnTo=%2Fthings%2F1gTyVIxaHSB-experiment-1&sharecode=Ri0EEm3LwM08j3dCpDki9pk6rcDBKoqTEt-b6Sd2Uzg

Exp3 
https://www.tinkercad.com/things/40fhuOna2A5-piezo-buzzer/editel?returnTo=https%3A%2F%2Fwww.tinkercad.com%2Fdashboard%2Fdesigns%2Fcircuits&sharecode=tJHK8j5pfO-fRByM0u3V86x0_VI6-JenZx7EVeWy5CA

Exp 4 - Series monitor
https://www.tinkercad.com/things/aFv4JnwAnQH/editel?sharecode=F8gr8qWmevinyIC3gf8dcuOXyEpICazmbyomDLTK8gw

Exp 5 Distance Measure
https://www.tinkercad.com/things/0y5oc7p9wUg-exp05-distance-measure/editel?returnTo=%2Fdashboard%2Fdesigns%2Fcircuits&sharecode=FhlN63nxoTFdTYS_pmu6XDhXIp6G4sa_kD_lT04LE8s

Exp 6 - Interfacing Temperature using Arduino
https://www.tinkercad.com/things/9FXIIDYbXZ1-amazing-wluff/editel?returnTo=https%3A%2F%2Fwww.tinkercad.com%2Fdashboard&sharecode=0RgrhV0NM-yq0fXGBE0L8KTJvb3eWL2L3jwiYamwUQk

Exp 7 - Interfacing Proximity Sensor
https://www.tinkercad.com/things/cF5YB8yhENg-sizzling-amberis/editel?returnTo=https%3A%2F%2Fwww.tinkercad.com%2Fdashboard%2Fdesigns%2Fcircuits&sharecode=TALNObAoclljOT-DNSgEIDug1KwlSLbLPi6LhH_RDr4

Exp 8 - . Interfacing and reading a potentiometer using Arduino
https://www.tinkercad.com/things/krtw1wS88ie-experiment-no-8/editel?sharecode=NHth4rj3tAthFh-hgegvGvzplqoyxBpeGaKbSOS9v94

Exp 9 - Push btn interface using Arduino
https://www.tinkercad.com/things/7exN8zfCPdO-glorious-bigery-crift/editel?returnTo=https%3A%2F%2Fwww.tinkercad.com%2Fdashboard&sharecode=Exk8ylh4PciomYni17940gDvyme5XO5p666nBEND_CM
![Glorious Bigery-Crift](https://github.com/user-attachments/assets/fccfb2ad-7488-4585-b34a-e8fba4061b5f)

--- EXP9 CODE --
// Pin configuration
const int buttonPin1 = 9; // Pin for 1st push button
const int buttonPin2 = 12; // Pin for 2nd push button
const int buzzerPin = 5; // Pin for the buzzer
const int ledPin = 13; // Pin for the LED (optional, for visual feedback)

// Variables to store the button states
int buttonState1 = 0; 
int buttonState2 = 0;

void setup() {
  // Initialize the serial monitor
  Serial.begin(9600);
  
  // Set the button pins as input
  pinMode(buttonPin1, INPUT);
  pinMode(buttonPin2, INPUT);
  
  // Set the buzzer and LED pins as output
  pinMode(buzzerPin, OUTPUT);
  pinMode(ledPin, OUTPUT);
}

void loop() {
  // Read the state of the push buttons
  buttonState1 = digitalRead(buttonPin1);
  buttonState2 = digitalRead(buttonPin2);
  
  // Check the state of the first push button
  if (buttonState1 == HIGH) {
    // Turn on the LED when button 1 is pressed
    digitalWrite(ledPin, HIGH);
    Serial.println("Button 1 Pressed: LED ON");
  } else {
    // Turn off the LED when button 1 is not pressed
    digitalWrite(ledPin, LOW);
    Serial.println("Button 1 Released: LED OFF");
  }

  // Check the state of the second push button
  if (buttonState2 == HIGH) {
    // Turn on the buzzer when button 2 is pressed
    digitalWrite(buzzerPin, HIGH);
    Serial.println("Button 2 Pressed: Buzzer ON");
  } else {
    // Turn off the buzzer when button 2 is not pressed
    digitalWrite(buzzerPin, LOW);
    Serial.println("Button 2 Released: Buzzer OFF");
  }

  delay(100); // Small delay for debounce
}
--- EXP9 CODE END ----


Exp 10 - Interfacing Light sensor LDR
https://www.tinkercad.com/things/ceXwJGjOi1O-/editel?returnTo=https%3A%2F%2Fwww.tinkercad.com%2Fdashboard&sharecode=ZVoooXIsnDcYqFYaj8e8W7SFyD7T5RPHZ0SQn2bEE08
