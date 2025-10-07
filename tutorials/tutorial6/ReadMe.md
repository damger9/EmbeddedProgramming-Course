# Tutorial 6 - Control Flow: The for, while, and do-while loop statements


## While

Example

```cpp
char country[] = "Netherlands";
int i = 0;

void setup() {
  // put your setup code here, to run once:
  Serial.begin(115200);  

  while(i<11){
    Serial.printf("%c", country[i]);
    Serial.println(country[i]);
    i++; // variable = variable+1; variable++;
  }
}

void loop() {
}


```

## Next Tutorial
Go to [Tutorial 7](../tutorial7/ReadMe.md) - Input and Output.

Back to [main page](../../README.md).