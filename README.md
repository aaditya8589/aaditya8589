- 👋 Hi, I’m Aaditya Agarwal
- 📫 This is simple python program to generate a password which includes numbers and letters.

import random
import string

def generate_password(length=12):

    characters = string.ascii_letters + string.digits
    
    # Randomly choose characters for the password
    password = ''.join(random.choice(characters) for i in range(length))
    
    return password

# User input for password length 
password_length = int(input("Enter password length (default 12): ") or 12)

# Generate and display the password
print(f"Generated password: {generate_password(password_length)}")
