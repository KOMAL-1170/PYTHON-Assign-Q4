# PYTHON-Assign-Q4
#(i)
import random
import string

for _ in range(100):
    length = random.randint(6, 8)
    rand_str = ''.join(random.choices(string.ascii_letters + string.digits, k=length))
    print(rand_str)

(ii)
def is_prime(n):
    if n < 2:
        return False
    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            return False
    return True

for num in range(600, 801):
    if is_prime(num):
        print(num)

#(iii)
for num in range(100, 1001):
    if num % 7 == 0 and num % 9 == 0:
        print(num)

