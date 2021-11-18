# Pythagorean Theorem (PYTHTHRM)
This program allows you to run Pythagorean theorem operations. It has two functions: [Find Hypotenuse](#find-hypotenuse), and [Find Side](#find-side). When the program is run, it will ask you to choose one of the functions. Both of these functions will be elaborated on in their own sections. 

Both functions can display the result as either a normal number, or as the square root of a number. For example, it is capable of displaying `√20` rather than `4.472135955`. This makes the calculator much more practical for solving Pythagorean theorem operations. Whether to display the result or the square root representation of the result is controlled by the following logic:

1. Calculate the result of the Pythagorean theorem operation.
2. If the result is an integer, display the result.
3. If the result is not an integer, but the square of the result is an integer, display the square root representation of the result.
4. If the result is not an integer, and the square of the result is not an integer, display the result.

In addition to this, `Ans` is set to the result of the operation, allowing math to be performed on the result without retyping.

## Find Hypotenuse
This function allows you to find the hypotenuse of a right triangle using the length of the other two sides. When run, the program will ask for the length of side one and side two. It will then output the length of the hypotenuse as the result.

This function uses the following formula to calculate the result, where `A` is the length of side 1, and `B` is the length of side 2:

```
sqrt( A^2 + B^2 )
```

## Find Side
This function allows you to find an unknown side of a right triangle using the length of the known side and the hypotenuse. When run, the program will ask for the length of the known side and the hypotenuse. It will then output the length of the unknown side as the result.

This function uses the following formula to calculate the result, where `A` is the length of the known side and `H` is the length of the hypotenuse:

```
sqrt( H^2 - A^2 )
```
