# pwdGenerator
from random import  *
from string import  *
import pyperclip as pyp

chars = []
chars.extend(ascii_letters)
chars.extend(digits)
chars.extend(punctuation)

no_of_pwd = int(input('Enter no.of passwords required: '))
pwd_len = int(input('Enter password(s) length: '))

for pwds in range(no_of_pwd):
	pwd = ''
	for ch in range(pwd_len):
		pwd = pwd + choice(chars)
	pyp.copy(pwd) 
	print(pwd)



	
