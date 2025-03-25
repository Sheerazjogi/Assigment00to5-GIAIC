Problem Breakdown:
In this problem, we want to create a system that checks if a user's entered password matches the stored password using hashing for security purposes. Rather than storing the actual password, we store a hashed version of the password, and when a user logs in, we hash the entered password and compare it to the stored hash. If they match, access is granted.

Key Concepts:
Hashing: We use a hash function (in this case, SHA-256) to convert a password into a fixed-size string of characters, which is a unique identifier for the password. This process makes the password secure since the hash cannot be easily reversed to obtain the original password.

SHA256 Hashing: We use Python’s hashlib.sha256() function to create a hashed version of the password. This function takes an input string (the password), encodes it into bytes, and returns a hash object which can be converted to a hexadecimal string representation.

Password Verification: To verify the password, the entered password is hashed, and the resulting hash is compared to the stored hash for the given email.

Code Walkthrough:
hash_password(password) function:

This function takes the input password, encodes it to bytes using .encode(), and hashes it using the SHA-256 algorithm. The result is then converted into a hexadecimal string using .hexdigest().

login(email, stored_logins, password_to_check) function:

This function checks whether the entered password matches the stored hash.

It looks up the hash of the password in stored_logins (a dictionary where the keys are email addresses and the values are the hashed passwords).

It compares the hash of password_to_check with the stored hash using the hash_password function.

main() function:

This is where the program's logic is run. We create a dictionary stored_logins with email keys and hashed password values.

Then, we call the login() function with different emails and passwords to see if the entered password matches the stored password hash.

Code:
python
Copy
from hashlib import sha256

def login(email, stored_logins, password_to_check):
    """
    Returns True if the hash of the password we are checking matches the one in stored_logins
    for a specific email. Otherwise, returns False.

    email: the email we are checking the password for
    stored_logins: a dictionary pointing from an email to its hashed password
    password_to_check: a password we want to test alongside the email to login with
    """
    
    # Compare the hash of the entered password with the stored hashed password
    if stored_logins[email] == hash_password(password_to_check):
        return True
    return False

# Hashing function
def hash_password(password):
    """
    Takes in a password and returns the SHA256 hashed value for that specific password.
    
    Inputs:
        password: the password we want
    
    Outputs:
        the hashed form of the input password
    """
    return sha256(password.encode()).hexdigest()

def main():
    # stored_logins is a dictionary with emails as keys and hashed passwords as values
    stored_logins = {
        "example@gmail.com": "5e884898da28047151d0e56f8dc6292773603d0d6aabbdd62a11ef721d1542d8",
        "code_in_placer@cip.org": "973607a4ae7b4cf7d96a100b0fb07e8519cc4f70441d41214a9f811577bb06cc",
        "student@stanford.edu": "882c6df720fd99f5eebb1581a1cf975625cea8a160283011c0b9512bb56c95fb"
    }
    
    # Testing the login function with different passwords
    print(login("example@gmail.com", stored_logins, "word"))  # False, hashed password doesn't match
    print(login("example@gmail.com", stored_logins, "password"))  # True, matches stored hash
    
    print(login("code_in_placer@cip.org", stored_logins, "Karel"))  # False, case-sensitive
    print(login("code_in_placer@cip.org", stored_logins, "karel"))  # False, incorrect case
    
    print(login("student@stanford.edu", stored_logins, "password"))  # False, incorrect password
    print(login("student@stanford.edu", stored_logins, "123!456?789"))  # False, incorrect password

if __name__ == '__main__':
    main()