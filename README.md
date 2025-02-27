# PHP Compiler Python Package

This Python package facilitates seamless compilation of PHP code through integration with the Codegyan API, streamlining the verification process and ensuring code correctness with minimal effort.

## Installation

You can install the package via pip:

```python
pip install php-compiler-py
```

## Usage

Before using the Pakage, you need to obtain an API key and client ID from Codegyan. Follow these steps to get your API credentials:

1. **Sign Up/Login**: If you don't have an account, sign up for a [Codegyan account](https://www.codegyan.in/). If you already have an account, log in to your dashboard.

2. **Get Credentials**: Once logged in, navigate to the [Developer Console](https://developer.codegyan.in/) or API settings in your account dashboard. Here, you will find your API key and client ID. Copy these credentials and use them when initializing the Pakage in your code.

Here's an example of how to initialize the Pakage with your API key and client ID:

- Import the compilePHP function from the package:

```python
from php_compiler_py import compilePHP
```

- Call the compilePHP function with your API key, client ID, and PHP code:

```python
apiKey = 'your_api_key'
clientId = 'your_client_id'
code = '<?php echo "Hello, world!"; ?>'

result = compilePHP(apiKey, clientId, code)
print(result)

```

Replace **'your_api_key'** and **'your_client_id'** with your actual API key and client ID obtained from the Codegyan website. Replace <?php echo "Hello, world!"; ?> with the code you want to compile.

The function will compile the provided PHP code using the Codegyan API and return the compilation result.

# Features

- **PHP Code Compilation :** The package provides a function `compilePHP(apiKey, clientId, code)` that allows users to compile PHP code using the Codegyan API. This feature enables developers to verify the correctness of their PHP code without the need for local PHP installations.

- **Simple Interface :** With just a few lines of code, users can easily integrate the `compilePHP` function into their Python projects. The function takes API key, client ID, and PHP code as arguments, making it straightforward to use.

- **Error Handling :** The package includes error handling to ensure robustness during compilation. If there are any issues with the compilation process, appropriate error messages are returned, allowing developers to identify and address problems effectively.

- **Customization Options :** Users have the flexibility to customize the compilation process by providing their own API key and client ID. This customization ensures that developers can utilize their Codegyan account for PHP code compilation seamlessly.

- **License :** The package is licensed under the MIT License, providing users with the freedom to use, modify, and distribute the code according to their requirements.

- **Compatibility :** The package is compatible with both Python 2 and Python 3, ensuring that a wide range of Python environments can utilize its functionality without compatibility issues.

## License

This project is licensed under the MIT License - see the **[License](https://opensource.org/licenses/MIT)** file for details.
