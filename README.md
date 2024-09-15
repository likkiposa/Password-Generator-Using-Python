# Password Generator in Python

This is a simple **password generator** script written in Python. It generates secure passwords of varying lengths, combining lowercase letters, uppercase letters, and numbers to ensure password strength.

## Features

- **Random Password Generation**: Generates random passwords using lowercase letters.
- **Uppercase and Number Replacement**: Automatically replaces some characters with uppercase letters and digits.
- **Customizable Length**: Users can input the number of passwords and the length of each password.
- **Ensures Minimum Length**: Passwords shorter than 3 characters are automatically adjusted to the minimum length.

## How It Works

The script generates passwords based on user input. For each password:
1. It selects random lowercase letters.
2. It replaces some characters with uppercase letters.
3. It replaces a few characters with numbers.
4. It returns a list of generated passwords, which are displayed to the user.

## How to Use

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/yourusername/password-generator-python.git
    cd password-generator-python
    ```

2. **Run the Script**:
    Run the script using Python:
    ```bash
    python password_generator.py
    ```

3. **Input the Number of Passwords**: 
   The script will ask you how many passwords you'd like to generate.
   
4. **Input the Length of Each Password**: 
   You can specify the desired length for each password. Passwords shorter than 3 characters will be automatically adjusted to the minimum length.

## Example

```bash
How many passwords do you want to generate? 2
Generating 2 passwords
Minimum length of password should be 3
Enter the length of Password #1 8
Enter the length of Password #2 5
Password #1 = a9cTdefg
Password #2 = jklMn
```

## Code Breakdown

- **`generatePassword(pwlength)`**: This function generates a list of passwords based on the input lengths. It builds a password by selecting random letters and replacing some with uppercase letters and numbers.
  
- **`replaceWithNumber(pword)`**: Replaces random characters in the first half of the password with digits.
  
- **`replaceWithUppercaseLetter(pword)`**: Replaces random characters in the second half of the password with uppercase letters.
  
- **`main()`**: The main function prompts the user for input (number of passwords and lengths), calls the `generatePassword` function, and displays the generated passwords.

## Requirements

- Python 3.x

## License

This project is licensed under the MIT License. Feel free to use and modify the code as per your needs.

