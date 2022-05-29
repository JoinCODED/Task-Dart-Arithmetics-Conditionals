1. You main method should look like this:

```dart
void main() {
  double tempInFahrenheit = 86;
}
```

2. Create another variable of type double and name of `tempInCelsius`:

```dart
void main() {
  double tempInFahrenheit = 86;
  double tempInCelsius = 0.0;
}
```

3. Start applying the formula:

```dart
void main() {
  double tempInFahrenheit = 86;
  double tempInCelsius = (tempInFahrenheit - 32) / 1.8;
}
```

4. Print out the result:

```dart
void main() {
  double tempInFahrenheit = 86;
  double tempInCelsius = (tempInFahrenheit - 32) / 1.8;
  print('${tempInFahrenheit}F = ${tempInCelsius}C');
}
```

### 🍋 Floats Methods

To show only 1 fractional digit we will use `toStringAsFixed()` method by passing it the number of fractional digits we want:

```dart
void main() {
  double tempInFahrenheit = 86;
  double tempInCelsius = (tempInFahrenheit - 32) / 1.8;
  print('${tempInFahrenheit}F = ${tempInCelsius.toStringAsFixed(1)}C');
}
```

### 🌶 Vice Versa

```dart
void main() {
  double tempInCelsius = 26;
  double tempInFahrenheit = tempInCelsius * 1.8 + 32;
  print('${tempInFahrenheit.toStringAsFixed(1)}F = ${tempInCelsius}C');
}
```

### 🍋 Conditionals❓

1. Your main method should look like this:

```dart
void main() {
int mark = 78;
}
```

2. Start with you first conditions:

```
if `mark` is more than or equal to 80
```

```dart
void main() {
int mark = 78;
if (mark >= 80){
    print("A");
}
}
```

3. Move to the next condition:

```
if `mark` is more than or equal to 70 and less than 80
```

let's translate that with code:

if: if

mark: mark

more than: >

or equal to: =

and: &&

less than: <

```dart
void main() {
int mark = 78;
if (mark >= 80){
    print("A");
} else if (mark >= 70 && mark < 80){
    print("B");
}
}
```

4. Do the same for the next conditions:

```dart
void main() {
int mark = 78;
if (mark >= 80){
    print("A");
} else if (mark >= 70){
    print("B");
} else if (mark >= 60){
    print("C");
} else if (mark >= 50){
    print("D");
}
}
```

5. And we use `else` for the last condition:

```dart
void main() {
int mark = 78;
if (mark >= 80){
    print("A");
} else if (mark >= 70){
    print("B");
} else if (mark >= 60){
    print("C");
} else if (mark >= 50){
    print("D");
} else {
    print("F");
}
}
```

### 🌶 More Practice: FizzBuzz

1. Your main method should look like this:

```dart
void main() {
int i = 9;
}
```

2. Our first condition is:

```
if i is divisible by 3 and 5
```

To know if a number is divisible by 3 we use the modula `%`.

```
if a number % 3 = 0 , then it's divisible by 3
```

Let's implement that in dart:

```dart
void main() {
int i = 9;
if (i % 3 == 0 && i % 5 == 0 ){
    print("fizz buzz");
} else if (i % 3 == 0){
    print('fizz');
} else if (i % 5 == 0){
    print('buzz');
} else {
    print(i);
}
}
```

### 🌶 Switch Case

```dart
void main() {
  int x = 5;
  int y = 5;
  String operation = "+";

  switch (operation) {
    case "*":
      print(x * y);
      break;
    case "+":
      print(x + y);
      break;
    case "-":
      print(x - y);
      break;
    case "/":
      print(x / y);
      break;
  }
}
```
