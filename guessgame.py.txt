




import random

case=1
y=1

rd=1
d=0
range_dif=0
for s in range(4):
	if case<4:
		print("guess the number between 1-200")

		number=input("enter that number")

		randnum=random.randint(1,200)

		
		for u in range(case):
			range_dif+=10
		modulo=randnum%10
		
		if modulo==0:
			rangeb=randnum
			rangea=randnum-range_dif
		else:
			rangea=randnum-modulo
			rangeb=rangea+range_dif
		
		
	
		for i in range(y-d):
			if y<6:
				if number==randnum:
		
					print("you won the game")

					case+=1	
				else:
		
					print(randnum)
		
					print("try again")
		
					print("you have only" ,5-y, "chances")
	
					print("hint:the number is between" ,rangea, "and" ,rangeb )
					y+=1
					d+=1
			if y==5:
				print("GAME OVERE")



