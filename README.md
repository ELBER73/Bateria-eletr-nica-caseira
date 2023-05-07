# Bateria-eletronica caseira com arduino mega
Código para montagem de bateria eletrônica caseira
Para você poder montar, se divertir e ainda tirar um som com as suas músicas preferir.

int buttonPin1 = 2;
int buttonPin2 = 3;
int buttonPin3 = 4;
int buttonPin4 = 5;
int buttonPin5 = 6;
int buttonPin6 = 7;

int buzzerPin = 8;

void setup() {
  pinMode(buttonPin1, INPUT_PULLUP);
  pinMode(buttonPin2, INPUT_PULLUP);
  pinMode(buttonPin3, INPUT_PULLUP);
  pinMode(buttonPin4, INPUT_PULLUP);
  pinMode(buttonPin5, INPUT_PULLUP);
  pinMode(buttonPin6, INPUT_PULLUP);

  pinMode(buzzerPin, OUTPUT);
}

void loop() {
  if (digitalRead(buttonPin1) == LOW) {
    tone(buzzerPin, 440);
    delay(250);
    noTone(buzzerPin);
  }

  if (digitalRead(buttonPin2) == LOW) {
    tone(buzzerPin, 494);
    delay(250);
    noTone(buzzerPin);
  }

  if (digitalRead(buttonPin3) == LOW) {
    tone(buzzerPin, 523);
    delay(250);
    noTone(buzzerPin);
  }

  if (digitalRead(buttonPin4) == LOW) {
    tone(buzzerPin, 587);
    delay(250);
    noTone(buzzerPin);
  }

  if (digitalRead(buttonPin5) == LOW) {
    tone(buzzerPin, 659);
    delay(250);
    noTone(buzzerPin);
  }

  if (digitalRead(buttonPin6) == LOW) {
    tone(buzzerPin, 698);
    delay(250);
    noTone(buzzerPin);
  }
}

