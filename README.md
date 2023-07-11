# CielAndReceipt
# cook your dish here
l = [2**p for p in range(12)]
t = int(input())
for i in range(t):
    x = int(input())
    c = 0
    for j in range(len(l),0,-1):
        c = c + x//l[j-1]
        x %= l[j-1]
    print(c)
