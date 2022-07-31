'''Write a program to find sum of following series using functions :
 1! + 2! + 3! + 4! +….. + n! '''

def fact(n):
    if (n == 0):
        return 1
    else:
        return n *fact(n-1)
def fact_sum(n):
    if (n == 0):
        return 0
    else:
        return fact(n) + fact_sum(n-1)
n = int(input("Enter a Number : "))

print("Factorial sum : ",fact_sum(n))

