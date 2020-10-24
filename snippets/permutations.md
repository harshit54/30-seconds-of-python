---

title: permutations

tags: utility, beginner, combinatorics

---
Calculates the number of ways of choosing r objects from n unique objects.

$^nP_r = \dfrac{n!}{(n-r)!}$

 - Calculates: $n!$, $(n-r)!$
 - Uses recursion for calculating factorial  

```py
def permutations(n, r):
	def factorial(num):
		if num <= 1:
			return 1
		else:
			return num*factorial(num-1)
	return factorial(n)/(factorial(n-r))
```

