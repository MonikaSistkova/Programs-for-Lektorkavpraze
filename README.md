# Programs-for-Lektorkavpraze

from sympy import symbols, Eq, solve
a,b = symbols('a b')
x1=int(input("Zadejte první souřadnici bodu A "))
y1=int(input("Zadejte druhou souřadnici bodu A "))
x2=int(input("Zadejte první souřadnici bodu B "))
y2=int(input("Zadejte druhou souradnici bodu B "))
eq1=Eq(a*x1+b-y1)
eq2=Eq(a*x2+b-y2)
solve((eq1,eq2), (a, b))
sol_dict = solve((eq1,eq2), (a, b))
print(f'a = {sol_dict[a]}')
print(f'b = {sol_dict[b]}')
