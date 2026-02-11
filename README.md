# sum-of-Fractions
from math import gcd

def fraction(num1, num2, de1, de2):
    numerator = (num1 * de2) + (num2 * de1)
    denominator = (de1 * de2)
    d = gcd(numerator, denominator)
    numerator //= d
    denominator //= d
    print(f"{numerator}/{denominator}")

num1 = int(input("Enter numerator of first fraction: "))
de1 = int(input("Enter denominator of first fraction: "))
num2 = int(input("Enter numerator of second fraction: "))
de2 = int(input("Enter denominator of second fraction: "))

fraction(num1, num2, de1, de2)