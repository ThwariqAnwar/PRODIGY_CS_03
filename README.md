# PRODIGY_CS_03

# 🔐 Secure Pass

This Python script evaluates the strength of a user-provided password based on its length, character variety, and whether it appears in a list of common passwords. The script assigns a strength score to the password, with a maximum score of 14.

## 🌟 Features

- **Password Length Check**: The script evaluates the length of the password and awards points for exceeding certain length thresholds.
- **Character Variety Check**: It checks for the presence of uppercase letters, lowercase letters, digits, and special characters, awarding points for using a mix of these types.
- **Common Password Detection**: The script checks the input password against a list of common passwords (from `common.txt`). If the password is found in this list, the score is automatically set to 0.
- **Score-Based Evaluation**: Based on the total score, the password is rated as `weak`, `average`, `good`, or `strong`.

## 🛠️ How It Works

1. **Input**: The script takes a password as input from the user.
2. **Character Analysis**:
   - Checks if the password contains:
     - Uppercase letters
     - Lowercase letters
     - Digits
     - Special characters
3. **Length Evaluation**: 
   - Awards points based on password length:
     - 2 points for length > 8
     - 2 points for length > 12
     - 2 points for length > 17
     - 2 points for length > 20
4. **Common Password Detection**: 
   - If the password matches any in the `common.txt` file, the score is automatically set to `0` and no further checks are done.
5. **Final Score**: 
   - The total score is calculated out of 14, and a corresponding rating is given (weak, average, good, or strong).

## 📊 Scoring Breakdown

- **Password Length**:
  - > 8 characters: +2 points
  - > 12 characters: +2 points
  - > 17 characters: +2 points
  - > 20 characters: +2 points
- **Character Variety**:
  - 2 or more types: +2 points
  - 3 or more types: +2 points
  - All 4 types: +2 points
- **Common Password Check**:
  - If found in `common.txt`: Score = 0

## 🧪 Example

Here’s an example of how the script works:

```bash
$ python password_checker.py
Enter the password: P@ssw0rd123!

Password length is 12, adding 4 points
Password has 4 different character types, adding 3 points!
Password is strong! score: 7 / 14
```

## 🚀 Getting Started

### Installation

1. Clone this repository:

   ```bash
   https://github.com/ThwariqAnwar/PRODIGY_CS_03.git
   ```
   
2. Ensure you have a `common.txt` file with a list of common passwords. You can use publicly available datasets for this purpose.

### Usage

Run the script and enter a password to evaluate its strength:

```bash
python securepass.py
```

## 📝 Notes

- The list of common passwords (`common.txt`) should be placed in the same directory as the script.
- Modify the `common.txt` file to include any additional passwords you want to flag as weak.

---

🎉 **Happy password securing!** 🔐

--- 
