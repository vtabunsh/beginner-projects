number = input("enter your number")
numlist = []
output = ""
if number < 0:
    number = number*-1
for i in range(1,(number+1)):
    remain = number%i
    if remain == 0:
        numlist.append(i)
        output = output + str(i) + ", "
    else:
        continue
output = output[:-2]
print output 
if len(numlist) == 2:
    print "prime number"
