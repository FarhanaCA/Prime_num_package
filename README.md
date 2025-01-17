# Prime Number Generator

## Overview

`prime_generator` is a Python package designed to provide comprehensive utilities for working with prime numbers. Whether you're doing mathematical research, solving coding challenges, or just exploring number theory, this package offers a range of functions to help you work with prime numbers efficiently.

## Installation

### Prerequisites
- Python 3.8+
- pip

### Install from Source
```bash
# Clone the repository
git clone https://github.com/yourusername/prime_generator.git

# Navigate to the project directory
cd prime_generator

# Install the package
pip install .
```

### Install for Development
```bash
# Install in editable mode with test dependencies
pip install -e .[test]
```

## Features

### Prime Number Checking
- Check if a number is prime
- Efficiently implemented with square root optimization

### Prime Number Generation
- Generate prime numbers within a specified range
- Flexible start and end parameters

### Advanced Prime Number Operations
- Find the nth prime number
- Compute prime factors of a number
- Count prime numbers in a given range

## Usage Examples

### Basic Prime Checking
```python
from prime_generator import is_prime

print(is_prime(17))  # True
print(is_prime(4))   # False
```

### Generating Prime Numbers
```python
from prime_generator import generate_primes

# Generate primes between 10 and 20
primes = generate_primes(10, 20)
print(primes)  # [11, 13, 17, 19]
```

### Finding Nth Prime
```python
from prime_generator import nth_prime

# Find the 5th prime number
print(nth_prime(5))  # 11
```

### Prime Factorization
```python
from prime_generator import prime_factors

# Get prime factors of 12
print(prime_factors(12))  # [2, 2, 3]
```

### Counting Primes in a Range
```python
from prime_generator import count_primes_in_range

# Count primes between 10 and 20
print(count_primes_in_range(10, 20))  # 4
```

## Error Handling

The package includes comprehensive error handling:
- Raises `ValueError` for invalid inputs
- Prevents operations on numbers less than 2
- Ensures range validity in generation methods

## Performance

- Optimized prime checking algorithm
- Linear time complexity for most operations
- Square root optimization for primality testing

## Running Tests

```bash
# Requires pytest
pytest tests/
```

## Contributing

### Reporting Issues
- Use GitHub Issues
- Provide clear, reproducible examples
- Specify your Python version

### Development Guidelines
1. Fork the repository
2. Create a feature branch
3. Write tests for new functionality
4. Ensure all tests pass
5. Submit a pull request

## Performance Considerations

- Best suited for small to medium-sized number ranges
- For extremely large prime number operations, consider specialized libraries

## License

MIT License

## Future Roadmap
- Support for large prime number generation
- More advanced prime number algorithms
- Additional statistical prime number functions

## Disclaimer

This package is intended for educational and computational purposes. Always verify critical mathematical computations.

## Acknowledgments

Inspired by the beauty of number theory and the joy of mathematical exploration.