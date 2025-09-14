# Password-generator-
A simple password generator which brings about suggestions to the user making it from random symbols, numbers and letters. Also length and symbols are included in it. 

CODE:
import random
import string

def generate_password(length=16, include_symbols=True):
    chars = [chr(i) for i in range(33, 127)]
    return ''.join(random.choices(chars, k=length))

password = generate_password()
print(password)
