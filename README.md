# Password-generator
import secrets
import string

def  password_gen(password_length):
    
    characters = string.ascii_letters + string.digits
    
    secure_passoword = ''.join(secrets.choice(characters) for i in range(password_length))
    
    return secure_passoword

def main():
    
    user_password_length = int(input("inputs number of digits for password: "))
    
    print("Password Generated: ", password_gen(user_password_length))
    
main()
