# strong-numbers-
strong numbers 
n = int(input())
temp = n
total = 0

while temp > 0:
    digit = temp % 10
    fact = 1

    for i in range(1, digit + 1):
        fact = fact * i

    total = total + fact
    temp = temp // 10

if total == n:
    print("Strong")
else:
    print("Not Strong")