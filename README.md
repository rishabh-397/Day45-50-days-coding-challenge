# Day45-50-days-coding-challenge

## 🧑‍⚖️ Problem 1: Find the Town Judge

### Problem:
Identify the town judge based on the trust relationships between `n` people.

### Conditions:
- Judge trusts nobody.
- Judge is trusted by everyone (except themselves).
- Only one such person can exist.

### Approach:
- Use an array `trust_score` of size `n + 1`.
- For each trust pair `[a, b]`, decrease `trust_score[a]`, increase `trust_score[b]`.
- The person with `trust_score == n - 1` is the judge.

### Example:
Input: n = 3, trust = [[1,3],[2,3]]  
Output: 3

---

## 🔡 Problem 2: Greatest Common Divisor of Strings

### Problem:
Find the largest string `x` that divides both `str1` and `str2`.

### Approach:
- If `str1 + str2 != str2 + str1`, return "".
- Otherwise, return `str1[0:gcd(len(str1), len(str2))]`.

### Example:
Input: str1 = "ABCABC", str2 = "ABC"  
Output: "ABC"

