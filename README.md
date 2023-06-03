# Assembly Code Project: Modulo, GCD, and Prime

This project contains assembly code that implements three essential operations: modulo calculation, greatest common divisor (GCD) calculation, and prime number determination. The code is designed to work with non-negative integer inputs and employs iterative and recursive approaches to perform the calculations.

## Modulo

The first subroutine, `modulo`, computes the modulo of two integer arguments without using multiplication or division instructions. It utilizes an iterative approach to iteratively subtract the divisor from the dividend until the dividend is less than the divisor. The resulting value is the modulo. The modulo subroutine can handle non-negative integers, assumes the divisor is not zero, and ensures that the result fits within a 64-bit register.

## GCD

The second subroutine, `gcd`, calculates the greatest common divisor between two integer arguments. It utilizes the `modulo` routine to compute the remainder iteratively. The GCD calculation is performed recursively by invoking the `gcd` subroutine with the second argument as the modulo of the two arguments. The recursion continues until the second argument becomes zero, at which point the first argument is returned as the GCD. Similar to the modulo routine, the GCD subroutine operates on non-negative integers and ensures the result fits within a 64-bit register.

## Prime

The third subroutine, `prime`, determines whether an integer argument is prime or not. It uses the `gcd` subroutine to check if the argument has any common divisors other than 1 and itself. If the GCD between the argument and any number other than 1 is greater than 1, the argument is not prime. The prime subroutine employs an iterative approach, but the specific details of the iteration are not provided in the project description. The subroutine assumes a non-negative integer input.

