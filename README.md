# Q.11
def is_palindrome(n):
   if n == 0:
       return True
   else:
       return (n % 10 == (int(is_palindrome(int(n/10))) % 10)) and is_palindrome(int(n/10))

num = 121

if is_palindrome(num):
   print(num, "is a palindrome number")
else:
   print(num, "is not a palindrome number")
