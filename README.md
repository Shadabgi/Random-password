# Random-password
import random
import string

pass_len = 12
charval = string.ascii_letters + string.digits + string.punctuation

#list comprehension method

password = "".join([random.choice(charval) for i in range(pass_len)])

#loop method 
password=""
for i in range(pass_len):
    password += random.choice(charval)

print("Your random password is :", password)
