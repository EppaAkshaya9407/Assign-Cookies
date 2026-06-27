# Assign-Cookies
g=list(map(int,input("Enter children's greed factors:").split()))
s=list(map(int,input("Enter cookie sizes:").split()))
r1=sorted(g)
r2=sorted(s)
i=0
j=0
n=len(r1)
m=len(r2)
while i<n and j<m:
    if r2[j]>=r1[i]:
        i+=1
    j+=1
print("Maximum content children:",i)
