# recurse_trampoline
# Example
def factorial(n):

     "Get factorial of n (trampolined)."
     
     if n <= 1:
     
         return 1
         
     return (yield factorial(n - 1)) * n


>>> print(trampoline(factorial(1000)))
