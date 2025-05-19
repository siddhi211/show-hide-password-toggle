
The PasswordInput component provides a password input field with a button that allows users to toggle between showing and hiding the password text. It manages both the password value and the visibility state using React hooks.

## How It Works (Step-by-Step)

1. **State Management**
**showPassword**: A boolean state that determines whether the password is visible (true for visible, false for hidden).
password: A string state that holds the current value of the password input.

2. **Password Input Field**
- The <input> field's type is set dynamically:
  - If showPassword is true, the type is "text" (password is visible)
  - If showPassword is false, the type is "password" (password is hidden)
- The input's value is controlled by the password state
- The onChange handler updates the password state as the user types

3. **Toggle Button**
- The <button> element controls password visibility by toggling the showPassword state on click
- The button's text content dynamically updates to display either "Show Password" or "Hide Password" based on current visibility state.

4. **Container**
The input and button are wrapped in a div with the class password-input-container for potential styling.

## Example User Flow
- User types a password: the input value updates
- User clicks "Show Password": the password becomes visible as plain text
- User clicks "Hide Password": the password is masked again

## Why This Is Useful
Improves user experience by allowing users to verify their password input.
Enhances accessibility and usability for password fields in forms.


The <input type="password"> HTML element creates a text field where the characters typed by the user are masked

![image](https://github.com/user-attachments/assets/2c4a282d-e065-47e9-b36b-0e44eae26d06)

