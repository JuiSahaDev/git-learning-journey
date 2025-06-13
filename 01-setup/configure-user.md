# Configure Git Username and Email

## 1. Set Username
Run the following commands in your terminal:
```bash
git config --global user.name "Your Name"
# Example:
git config --global user.name "Jui Saha"
```

## 2. Set email
Run this command:
```bash
git config --global user.email "your.email@example.com"
# Example:
git config --global user.email "officialjuisaha@gmail.com"
```

## 3. Verify configuration
To check your configured username and email, run:
```bash
git config --global --list
git config user.name
git config user.email
```