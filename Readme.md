# BigInteger Implementation in Java

## Overview
This is a custom implementation of a BigInteger library in Java, named **BigNumber**. The library provides support for performing arithmetic operations on large integers with arbitrary precision. It is capable of handling numbers that exceed the range of primitive data types in Java.

## Features
- Addition, subtraction, multiplication, and division of arbitrarily large integers
- Modulo and power operations
- Comparison methods (greater than, less than, equal to)
- Prime factorization and primality testing
- Random prime number generation
- Clean input method to handle leading zeros and spaces in input numbers

## Usage

### Creating a BigNumber
You can create a BigNumber instance using one of the following constructors:

1. From a **String** representation of a number:
```
BigNumber num1 = new BigNumber("12345678901234567890");
```
2. From a **long** value:
```
BigNumber num2 = new BigNumber(98765432109876543210L);
```

### Basic Arithmetic Operations
```
BigNumber sum = num1.add(num2);
BigNumber difference = num1.subtract(num2);
BigNumber product = num1.multiply(num2);
BigNumber quotient = num1.divide(num2);
BigNumber modulo = num1.mod(num2);
BigNumber power = num1.pow(3);
```

### Comparison Operations
```
boolean isEqual = num1.equals(num2);
boolean isGreater = num1.isGreaterThan(num2);
boolean isLess = num1.isLessThan(num2);
```

### Prime Factorization
```
ArrayList<BigNumber> primeFactors = num1.primeFactorization();
```

### Primality Testing
```
boolean isPrime = num1.isPrime(10);
```

### Random Prime Number Generation
```
BigNumber randomPrime = BigNumber.primeGenerator(50);
```

## Notes
- The library includes methods for handling sign (positive/negative) of the numbers.
- The **primeGenerator** method generates random prime numbers of a specified length using the Rabin-Miller primality test.
- For division operations, the **simpleDivide** method uses a basic long division approach.
- The library performs arithmetic operations in a straightforward manner and may not be optimized for extremely large numbers or high-performance requirements.

## Contact
If you have any questions or suggestions, please feel free to contact the developer at email@example.com.

**Happy computing with BigNumber!**