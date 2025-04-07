# Command-Line Calculator in C

This is a simple interactive calculator program written in C that supports basic arithmetic operations, modulus, exponentiation, and square roots. It allows continuous usage by reusing the previous result in subsequent calculations.

## Features

- Basic arithmetic: `+`, `-`, `*`, `/`
- Modulus: `%`
- Power: `^`
- Square root: `r`
- Reuse the previous result
- Graceful exit: `q`

## How to Compile

Use `gcc` or any C compiler of your choice:

```bash
gcc calculator.c -o calculator -lm
```

> The `-lm` flag links the math library required for `sqrt()` and `pow()`.

## How to Run

```bash
./calculator
```

## Usage

- The program prompts for an operator.
- For arithmetic operations, you will be asked to enter two numbers.
- For square root (`r`), only one number is needed.
- The result is stored and can be used in the next operation.
- Enter `q` to quit the program.

## Example

```
Enter an operator (+, -, *, /, %, ^, r for square root, q to quit): +
Enter the first number: 5
Enter the second number: 3
Result: 8.00

Enter an operator (+, -, *, /, %, ^, r for square root, q to quit): *
Using previous result as the first number: 8.00
Enter the second number: 2
Result: 16.00
```

## Notes

- Division by zero and modulus by zero are handled with error messages.
- Square root of negative numbers is not allowed and triggers an error message.
- Only integer inputs are valid for modulus operation.

## License

This project is released under the MIT License.
