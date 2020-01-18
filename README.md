# mi_testprogram
import random

x = 100  #int(input ("Введите число которое будет окончанием диапазона"))

number = int(input ("Введите число которое будет угадывать компьютер в введенном диапазоне"))
guess = 0
mi_random = 0
s = 0
while number != mi_random:
	s += 1
	mi_random = random.randint(guess, x)

	if mi_random > number:
		x = mi_random
		print(x)
	if mi_random < number:
		guess = mi_random
		print(guess)

print ("Решено за :", s, 'ваше число :', number)
