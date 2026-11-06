from math import isqrt

def digit_sum(n):
    return sum(int(ch) for ch in str(n))

def divisor_count(n):
    count = 0
    for d in range(1, isqrt(n) + 1):
        if n % d == 0:
            count += 1 if d*d == n else 2
    return count

solutions = []

for n in range(1,5185):
    s = digit_sum(n)
    tau = divisor_count(n)

    if n == s * tau:
        solutions.append((n,s,tau))

print(solutions)
