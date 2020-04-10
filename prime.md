from math import sqrt
 def prime(num):
	number=[]
	prime_number=[]
	for i in range(0,num):
		number.append(True)
	number[0]=False
	number[1]=False
	for i in range(0,num):
		for j in range(2,int(math.sqrt(i))+1):
			if i%j ==0:
				number[i]=False
	for i in range(0,num):
		if number[i]:
			prime_number.append(i)
	print(prime_number)
prime(100)
###[2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89, 97]
