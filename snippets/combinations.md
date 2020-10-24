---

title: combinations

tags: utility, beginner, combinatorics

---
Calculates the number of ways of choosing r objects from n unique objects.

$^nC_r = \dfrac{n!}{r! \cdot (n-r)!}$

 - Calculates: $n!$, $r!$ & $(n-r)!$
 - Uses recursion for calculating factorial  

```py
def combinations(n, r):
	def factorial(num):
		if num <= 1:
			return 1
		else:
			return num*factorial(num-1)
	return factorial(n)/(factorial(r)*factorial(n-r))
```

