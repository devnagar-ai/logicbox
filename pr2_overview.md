# pr2 Notebook Overview

This notebook contains a small interactive Python program. It runs in a loop and lets the user choose between two simple tasks: generating a text pattern or analyzing a range of numbers.

## What the code does

1. It shows a menu with three options:
   - Generate Pattern
   - Analyze Numbers
   - Exit

2. The user enters a choice.

3. Based on the choice, the program either:
   - prints a right-angled triangle made of asterisks, or
   - checks each number in a range and prints whether it is even or odd, then adds up the numbers.

4. The loop continues until the user chooses to exit.

## How the pattern generation works

When the user selects option `1`, the program asks for the number of rows.

Then it uses a `for` loop from `1` to the given row count. In each iteration it prints a line made of asterisks (`*`). The number of asterisks grows by one each row, which creates a simple triangle shape.

Example for 4 rows:
```
*
**
***
****
```

## How the number analysis works

When the user selects option `2`, the program asks for a starting number and an ending number.

It then loops through every integer in that range, inclusive. For each number it:
- checks if it is even using `num % 2 == 0`
- prints `Even` or `Odd`
- adds the number to a running total

After the loop finishes, it prints the sum of the numbers in the range.

## Exit and invalid input handling

- If the user chooses `3`, the program prints `Goodbye!` and breaks out of the loop.
- If the user enters anything else, it prints `Invalid choice` and shows the menu again.

## Notes

- The program uses `input()` for interaction, so it is intended to run with a console or terminal.
- It is deliberately straightforward and easy to follow.
