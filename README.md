# vaibhavi.

def AND(a,b,c): 
 return a&b&c
 
def OR(a,b): 
 return a|b
def NOT (a):
 return int(not a)
def NOR(a,b): 
 ans = OR(a,b)
 return NOT(ans)
j = int(input("Enter value of J = "))
k = int(input("Enter value of K = "))
Qp = int(input("Enter value of Previous Output = "))
r = AND(k,Qp,1)
s = AND(j,NOT(Qp),1)
a1 = NOR(s,Qp)
Qn = NOR(r,a1)
print("value of Next Output is = ",Qn)
