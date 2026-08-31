# README Audit

## README Fact-Check Table

| Claim Made in README | True? | Evidence / Correction Made |
|---|---|---|
| Program calculates factorial | Yes | `fact` is multiplied by each value inside the `for` loop. |
| Program calculates factorial of a user-entered number | No | `n = 5` is fixed in the code. No user input is taken. |
| Program accepts input from the terminal | No | There is no `input()` function in the program. Claim deleted. |
| Program can calculate factorial of any positive integer entered by the user | No | Current program only calculates factorial for fixed value `5`. Claim corrected. |
| Program validates negative numbers | No | There is no condition such as `if n < 0`. Claim deleted. |
| Program handles invalid input | No | There is no user input and no `try/except` handling. Claim deleted. |
| Python 3 is required | Yes | The file is a Python script and can be run using Python 3. |
| NumPy is required | No | There is no `import numpy` statement. NumPy is not used. Removed from requirements. |
| `requirements.txt` is required | No | No `requirements.txt` file exists in the repository. Installation instruction deleted. |
| Program can be run using `python factorial.py` | Yes | `factorial.py` is a standalone Python script. |
| Program displays `Enter a number: 5` | No | The program does not prompt the user. It only prints the result. |
| Output is `120` when `n = 5` | Yes | `5 × 4 × 3 × 2 × 1 = 120`. |
| Program uses a loop | Yes | The program uses `for i in range(1, n + 1)`. |
| Program uses multiplication to calculate factorial | Yes | `fact = fact * i` performs repeated multiplication. |
| Initial factorial value is `1` | Yes | The code contains `fact = 1`. |
| Program has input validation | No | No validation conditions exist. Claim deleted. |
| Program has error handling | No | No `try`, `except`, or other error-handling logic exists. |
| Program uses external Python libraries | No | No external libraries are imported. |
| Project uses MIT License | No | No `LICENSE` file exists in the repository. Licence section removed. |
| `pip install -r requirements.txt` is a valid installation step | No | No dependency file exists and no external packages are required. Command removed. |
| Project contains a factorial calculator | Yes | `factorial.py` calculates factorial of the fixed value `5`. |

---

## Corrections Made to the README

The following incorrect claims were removed or corrected:

- Removed the claim that the program accepts user input.
- Removed the claim that the program works for any user-entered positive integer.
- Removed negative-number validation.
- Removed invalid-input handling.
- Removed NumPy from the requirements.
- Removed the `pip install -r requirements.txt` instruction.
- Removed the fake `Enter a number:` prompt.
- Removed the MIT License claim.
- Corrected the description to state that the current value of `n` is fixed at `5`.
- Kept the verified output as `120`.

---

## Verified Program Behaviour

The actual program:

1. Sets `n = 5`.
2. Initializes `fact = 1`.
3. Uses a `for` loop from `1` to `n`.
4. Multiplies `fact` by each value of `i`.
5. Prints the final result.

Expected output:

```text
120
