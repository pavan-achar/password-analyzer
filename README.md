# Password Strength Checker (Python)

## Objective

Build a tool in Python that checks password strength based on a set of rules and provides
actionable feedback to improve passwords.

## Files
[password_checker.py](https://github.com/user-attachments/files/22505869/password_checker.py) : The main CLI and library.

## Rules & Scoring

The checker evaluates:

- Length (recommended >= 12 for best score)
- Character variety (lowercase, uppercase, digits, special characters)
- Avoid common passwords
- Avoid repeated sequences (e.g., 'abab', 'aaaa')
- Avoid sequential characters of length 3 (e.g., 'abc', '321')
- Entropy estimate (Shannon entropy)

Scoring assigns points for length, variety, and entropy, and deducts for weak patterns.

## Usage

Run from terminal:
```bash
python3 password_checker.py <password1> [password2 ...]
```
Or run interactively:
```bash
python3 password_checker.py
Enter password to check (or blank to exit):
```

## Output
<img width="1393" height="405" alt="Screenshot 2025-09-24 092611" src="https://github.com/user-attachments/assets/ec161305-7ccb-40b0-9797-8501810b06e0" />

## Integration

Import `score_password` from `password_checker.py` in other Python scripts to use programmatically.

## Notes

- This tool is educational. For real-world password guidance, combine this with policy checks
  (e.g., banned password lists, breach databases), and consider using proven password managers.
