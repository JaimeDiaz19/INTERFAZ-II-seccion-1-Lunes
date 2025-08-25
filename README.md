# INTERFAZ-II-seccion-1-Lunes
------------------------------------------------

#####  Ejercicio n° 1  : Hola Mundo!

``` js

void setup() {
  Serial.begin(9600); // Inicia la comunicación serie a 9600 bps
  Serial.println("Hola, Mundo!"); // Envía "Hola, Mundo!" al monitor serie
}

void loop() {
  // No es necesario poner nada en el loop para este ejemplo
}

```
#### Ejercicio n°2 : Led Intermitente (Blink)

```js
// C++ code
//
void setup()
{
  pinMode(13,OUTPUT);
  pinMode(8,OUTPUT);
  pinMode(LED_BUILTIN, OUTPUT);
}

void loop()
{
  digitalWrite(13, HIGH);
  
  delay(500); // Wait for 1000 millisecond(s)
  digitalWrite(8, HIGH);
  delay(200); // Wait for 1000 millisecond(s)
  digitalWrite(13,LOW);
  delay(800); 
  digitalWrite(8, LOW) ;
  
  delay(90); 
  
  
}

```
<img  Img/blinker.png > Led Parpadeante </a>

#### Ejercicio n°3 :Control Pulsador
```js
void setup() {
  pinMode(2, INPUT);  // Botón como entrada
  pinMode(13, OUTPUT);
}
void loop() {
  if (digitalRead(2) == HIGH) {  // Si se presiona el botón
    digitalWrite(13, HIGH);
  } else {
    digitalWrite(13, LOW);
  }
}

```


#### Ejercicio n°4 :  Potenciómetro

```js
void setup() {
  pinMode(9, OUTPUT);  // Pin PWM (símbolo ~)
}
void loop() {
  int valor = analogRead(A0);           // Leer potenciómetro (0-1023)
  int brillo = map(valor, 0, 1023, 0, 255);  // Convertir a rango PWM
  analogWrite(9, brillo);               // Ajustar brillo
}

```


#### Ejercicio n°5:





