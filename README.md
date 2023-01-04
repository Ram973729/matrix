# matrix
n=int(input())
m=[]
sum1=[]
sum2=[]
for i in range(n):
    l=[]
    for j in range(n):
        x=int(input())
        l.append(x)
    m.append(l)
for i in range(0,n):
    for j in range(0,n):
        if i==j:
            sum1.append(m[i][j])
        if i+j==n-1:
            sum2.append(m[i][j])
sum=sum1+sum2
print(max(sum))
