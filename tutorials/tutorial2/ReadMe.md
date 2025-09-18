# Tutorial 2 - Input and Output

## Learning Objectives

- Understand the concept of GPIO (General Purpose Input/Output).
- Configure ESP32 digital pins as input and output.
- Write simple programs to control LEDs.
- Read the state of physical buttons and use them to interact with LEDs.
- Develop basic conditional control logic using if/else statements.

## Introduction to GPIOs

==What are digital input and output pins==

==Basic configuration in code==

## Output Examples – LEDs

### Turning a single LED on and off

```cpp
// Turn on an LED using ESP32

// Define the pin where the LED is connected
const int ledPin = 23;

void setup() {
  // Initialize the LED pin as an output
  pinMode(ledPin, OUTPUT);

  // Turn the LED on
  digitalWrite(ledPin, HIGH);
}

void loop() {
  // Nothing else to do in the loop since the LED remains on
}
```

- `const int`: Declares the variable (`ledPin`) as a constant integer.
- `pinMode`: Initializes the pin as `INPUT` or `OUTPUT`. This allows the pin to send/write voltage to the LED (OUTPUT) or to receive/read (INPUT).
- `digitalWrite`: Sets the output of the pin to `HIGH` or `LOW`.

<details>
<summary>Exercise 1</summary>

**Task:**  
Develop a program to light up multiple LEDs.

**Hints:**  

- Use `pinMode()` to configure each LED pin as `OUTPUT`.  
- Use `digitalWrite()` to control the state of each LED.  
- Try to make them blink in sequence for extra practice (use the `delay()` function).  

**Solution:**  
[ex1](ex1/ex1.ino)
</details>

<details>
<summary>Exercise 2</summary>

**Task:**  
Develop a program to light up multiple LEDs. Make them blink in sequence (use the `delay()` function).  

**Solution:**  
[ex2](ex2/ex2.ino)

</details>

## Input Examples – Buttons

Reading the state of a button

Turning on an LED when the button is pressed

Combinations: multiple buttons controlling LEDs

## Input/Output Integration

Practical exercise: button as an LED toggle switch

Practical exercise: button selects which LED to turn on

## Exercises



## Next Tutorial
Go to [Tutorial 3](../tutorial3/ReadMe.md) - Input and Output.

Back to [main page](../../README.md).
