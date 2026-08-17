# 🛒 Shopping Cost Calculator

A simple Java console application that calculates the total cost of purchasing a chosen item based on price and quantity.

## 📋 Description

This program prompts the user to enter an item name, its price per unit, and the quantity they wish to buy. It then calculates and displays the total cost.

## ✨ Features

- Accepts any item name as input
- Calculates total cost based on price × quantity
- Displays a clean, formatted summary of the purchase
- Simple and beginner-friendly console interface

## 🚀 How to Run

1. Make sure you have Java installed (JDK 8 or higher)
2. Save the code in a file named `main.java`
3. Compile the program:
   ```bash
   javac main.java
   ```
4. Run the program:
   ```bash
   java main
   ```

## 💻 Example Usage

```
what item would you liketo buy? Notebook
Notebook
what is the price of the item?..., for each 2.50
how many would you like to buy? 4

you have bought4 Notebook/s
your Total cost: $10.0
```

## 🛠️ How It Works

1. `Scanner` reads user input from the console
2. The user enters the item name, price per unit, and quantity
3. `total` is calculated as `price * quantity`
4. The result is printed with a `$` currency symbol

## ⚠️ Known Bug (Fix Before Running)

The import statement currently has a stray space and **will not compile**:

```java
import java .util.Scanner;   // ❌ won't compile
```

Fix it by removing the space:

```java
import java.util.Scanner;    // ✅ correct
```

## 🔧 Possible Improvements

- Fix spacing/grammar in prompts (e.g. "would you liketo buy" → "would you like to buy")
- Add a space after "you have bought" and before the quantity for cleaner output
- Format `total` to 2 decimal places using `String.format("%.2f", total)` so `$10.0` displays as `$10.00`
- Add input validation (e.g. reject negative prices or quantities)
- Support multiple items in a single session (loop until user says "done")
- Let the user choose their currency symbol

## 📄 License

Free to use and modify for learning purposes.
