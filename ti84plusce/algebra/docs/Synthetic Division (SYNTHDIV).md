# Synthetic Division (SYNTHDIV)
The SYNTHDIV program allows you to perform synthetic division on your calculator. It requires an input in the form of list `L1` see [usage](#usage), and will overwrite lists `L2` and `L3`. The program has a non-interactive mode that allows it to be used seamlessly by other programs. See [non-interactive mode](#non-interactive-mode) for more details.

## Usage
Enter the polynomial you want to divide by setting the list `L1` to its coefficients. For example, for the polynomial `x³-2x²-8x-35`, you would set `L1` equal to `{1, -2, -8, -35}`. You can edit lists by pressing `stat -> Edit`.

![Entering a polynomial using the list editor](https://user-images.githubusercontent.com/47395245/142460124-3d5af2d5-4938-42e9-b689-a1d3c7a2dc32.png)

Once the polynomial is entered, run the SYNTHDIV program. The program will ask you what number you want to divide by. This is the number that would go on the left side during synthetic division. For example, to divide by `(x-5)`, you would enter `5`.

The program then performs synthetic division on the polynomial in `L1`, and outputs the results. The results are a list in the form `{x, x, x...}`. This list is the coefficients of a polynomial (similar to entering a polynomial), but the final value represents the remainder of the synthetic division. For example, a result of `{1, 3, 7, 0}` would be the polynomial `x²+3x+7` with a remainder of 0. See the [results](#results) section for more details.

## Results
The SYNTHDIV program performs synthetic division in the same way a human does and its output is correlated to the human method of synthetic division. `L1` contains the coefficients of the polynomial to divide by. This information is entered by the user, and can be correlated to the top row in synthetic division. `L2` is the second row of numbers in synthetic division, and `L3` is the bottom row that contains the result. (`L3` is the list that is displayed as output when running the program, but the full output of all lists can be viewed in the list editor.) The number to divide by, which is inputted by the user, is correlated to the number on the left of synthetic division. The images below show how the program's output correlates to synthetic division:

![Normal synthetic division](https://user-images.githubusercontent.com/47395245/142465947-f11f2a75-4861-4953-a6ef-00aa9d77a631.jpeg)

![The program's output](https://user-images.githubusercontent.com/47395245/142465615-e881088b-436b-42f8-98ab-2e469c4e4c9a.png)

## Non-Interactive Mode
The program has non-interactive mode that allows it to be used by other programs without outputting any text or requiring any user input. It will calculate using the contents of `L1`, and set `L2` and `L3`. The number to divide by will need to be set externally by setting `A` since the program will not ask for user input.

In order to enable non-interactive mode, set `Z` to `1` before running the program. When the program completes, it will reset `Z` to 0.

# Supported Calculators
This program supports the following calculators:
- TI-83
- TI-83 PCE
- TI-83 Plus
- TI-84
- TI-84 Plus
- TI-84 Plus CSE
- TI-84 Plus CE *(Tested)*

## Compatibility Issues
This program has no obvious compatibility issues with any TI-83 or TI-84 series calculators. However it should be noted that it has only been tested on the TI-84 Plus CE. If you encounter errors while using one of the supported calculators, please report a bug using the issue tracker.

