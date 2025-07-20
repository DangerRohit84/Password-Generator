# Password Generator (C Language)

## How the Program Works

###  Objective  
The goal of this program is to generate strong, random passwords of a user-defined length using a mix of uppercase letters, lowercase letters, digits, and special characters (optional).

---

## Setup

- Command-line based C program.
- Prompts the user to:
  - Enter desired password length.
  - Choose whether to include special characters.
- Outputs a randomly generated password based on selected criteria.

---

## Functionality

### Password Length:
- User inputs the number of characters the password should have.
- A minimum length of 1 is required.

### Character Sets:
- Digits: `0-9`
- Uppercase: `A-Z`
- Lowercase: `a-z`
- Special Characters: `@ # $ !` *(optional)*

### Randomization:
- Uses `rand()` and `srand(time(0))` to ensure different output every time.
- Random characters are picked from the allowed character pool based on user choice.

---

## Output

- Displays the generated password on the console.

#### Example:
```
Enter Length of your password: 10
Do you want Special character 
1.Yes
2.No
1
Generated Password: 3AYu2@Z9rb
```

---

## Features

- User-friendly input prompts
- Option to include/exclude special characters
- Clean output display
- Simple and fast execution

---

## Future Improvements

- Enforce inclusion of at least one character from each selected category
- Add password strength indicator
- Allow saving passwords to a text file
- Implement command-line flags (e.g., `--length 12 --specials`)

---

## Installation & Usage

### Requirements
- A C compiler (e.g., GCC)
- Compatible with Linux, macOS, or Windows terminal

### Steps to Compile and Run

1. **Save the source code as `password_generator.c`**
2. **Open terminal or command prompt**
3. **Compile the program**  
   ```bash
   gcc password_generator.c -o password_generator
   ```
4. **Run the executable**  
   ```bash
   ./password_generator
   ```

---
