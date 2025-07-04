# javascript-series
JavaScript series for learning

-------------------------------------------------------

Here’s a complete **list of questions to prepare for a machine round + full technical interview**, tailored especially for roles like **PHP/Laravel Backend Developer**, **Full Stack Developer**, or **Web Developer**—and based on companies like **Webkul**.

---

## 🧠 **Core Machine Round Topics (Coding & Logic)**

### 🔹 **Pattern Printing**

1. Print pyramid/star patterns with input validation.
2. Create symmetrical shapes using `@`, `*`, or numbers.
3. Print a diamond, hourglass, or Z-shape pattern.
4. Print Pascal's Triangle.
5. Numeric pyramid (e.g., 1, 121, 12321).

---

### 🔹 **Array & String Problems**

6. Find duplicate and missing elements in an array.
7. Reverse a string without using built-in functions.
8. Check if a string is a palindrome.
9. Rotate array left/right by k positions.
10. Longest substring without repeating characters.
11. Merge and sort two arrays manually.
12. Count frequency of elements in an array.

---

### 🔹 **Mathematical / Logical Questions**

13. Check if a number is prime.
14. Find factorial (with and without recursion).
15. Fibonacci series.
16. Count the number of digits or set bits.
17. Reverse digits of a number.
18. Sum of digits of a number.

---

### 🔹 **Recursion & Backtracking**

19. Tower of Hanoi problem.
20. Generate all subsets of a string/array.
21. Print all permutations of a string.
22. Solve a maze problem (backtracking).
23. Recursive binary search.

---

### 🔹 **Sorting & Searching**

24. Implement bubble, selection, and merge sort.
25. Write binary search without built-in functions.
26. Kth largest or smallest number in an array.
27. Search for a specific value in a matrix.

---

## 🧩 **PHP/Laravel Backend Questions**

### 🔹 **PHP Fundamentals**

28. Difference between `include`, `require`, `require_once`.
29. What is a closure or anonymous function?
30. PHP data types, arrays, and string functions.
31. How to handle sessions and cookies?
32. Difference between `==` and `===` in PHP.
33. How does error handling work (`try-catch`)?

---

### 🔹 **OOP in PHP**

34. Define abstraction, inheritance, and polymorphism.
35. Interface vs Abstract Class.
36. What is a constructor and destructor?
37. Singleton Design Pattern in PHP.
38. Traits vs Interfaces.
39. Magic methods in PHP (`__get`, `__set`, `__call`, etc.)

---

### 🔹 **Laravel Framework**

40. Laravel folder structure explanation.
41. What are migrations and seeders?
42. Explain route model binding.
43. How to use relationships (`hasOne`, `hasMany`, etc.)?
44. Difference between `pluck()`, `select()`, `get()` and `first()`.
45. Middleware in Laravel—what and why?
46. Events and Listeners in Laravel.
47. Laravel service container and facades.
48. What are queues and jobs in Laravel?
49. Artisan commands — how to create and use?

---

### 🔹 **Database (SQL / MySQL)**

50. Query for 2nd highest salary.
51. Difference between `WHERE` and `HAVING`.
52. JOINs: `INNER`, `LEFT`, `RIGHT`, `FULL`.
53. GROUP BY and aggregate functions (COUNT, SUM).
54. Subqueries and nested SELECT.
55. Create table with constraints (foreign key, unique).

---

### 🔹 **API / JSON**

56. What is REST API? Explain its verbs (`GET`, `POST`, etc.)
57. How to return JSON in Laravel.
58. Difference between `PUT` and `PATCH`.
59. How to validate incoming JSON using Laravel?
60. How to handle API authentication using tokens (Passport/Sanctum)?

---

### 🔹 **HTML / JS (if Full Stack role)**

61. Create dynamic form fields using jQuery.
62. Explain event bubbling in JS.
63. What is AJAX and how does it work?
64. Use localStorage and sessionStorage.
65. Validate form using JavaScript.

---

## ✅ **Bonus: Real-Time/Project Questions**

66. Explain a recent project you’ve worked on.
67. How do you debug in Laravel?
68. How do you optimize a slow query?
69. What is rate limiting in APIs and how to implement it?
70. Explain version control (Git basics: pull, merge, branch).

---

Here are **20 PHP pattern programs** commonly asked in interviews. You can copy and run them directly in any PHP environment.

---

### ✅ 1. Left-Aligned Triangle

```php
for($i = 1; $i <= 5; $i++) {
    echo str_repeat("*", $i) . "\n";
}
```

---

### ✅ 2. Right-Aligned Triangle

```php
for($i = 1; $i <= 5; $i++) {
    echo str_repeat(" ", 5 - $i) . str_repeat("*", $i) . "\n";
}
```

---

### ✅ 3. Pyramid

```php
for($i = 1; $i <= 5; $i++) {
    echo str_repeat(" ", 5 - $i) . str_repeat("* ", $i) . "\n";
}
```

---

### ✅ 4. Inverted Left Triangle

```php
for($i = 5; $i >= 1; $i--) {
    echo str_repeat("*", $i) . "\n";
}
```

---

### ✅ 5. Inverted Right Triangle

```php
for($i = 5; $i >= 1; $i--) {
    echo str_repeat(" ", 5 - $i) . str_repeat("*", $i) . "\n";
}
```

---

### ✅ 6. Diamond Pattern

```php
$n = 5;
for($i = 1; $i <= $n; $i++) {
    echo str_repeat(" ", $n - $i) . str_repeat("* ", $i) . "\n";
}
for($i = $n - 1; $i >= 1; $i--) {
    echo str_repeat(" ", $n - $i) . str_repeat("* ", $i) . "\n";
}
```

---

### ✅ 7. Half Diamond

```php
$n = 5;
for($i = 1; $i <= $n; $i++) echo str_repeat("*", $i) . "\n";
for($i = $n - 1; $i >= 1; $i--) echo str_repeat("*", $i) . "\n";
```

---

### ✅ 8. Number Pyramid

```php
for($i = 1; $i <= 5; $i++) {
    for($j = 1; $j <= $i; $j++) echo $j;
    echo "\n";
}
```

---

### ✅ 9. Floyd’s Triangle

```php
$count = 1;
for($i = 1; $i <= 5; $i++) {
    for($j = 1; $j <= $i; $j++) echo $count++ . " ";
    echo "\n";
}
```

---

### ✅ 10. Pascal's Triangle

```php
function fact($n) {
    return ($n <= 1) ? 1 : $n * fact($n - 1);
}
for($i = 0; $i < 5; $i++) {
    for($j = 0; $j <= $i; $j++) {
        echo fact($i) / (fact($j) * fact($i - $j)) . " ";
    }
    echo "\n";
}
```

---

### ✅ 11. Binary Triangle

```php
for($i = 1; $i <= 5; $i++) {
    for($j = 1; $j <= $i; $j++) echo $j % 2;
    echo "\n";
}
```

---

### ✅ 12. Hollow Square

```php
$n = 5;
for($i = 1; $i <= $n; $i++) {
    for($j = 1; $j <= $n; $j++) {
        echo ($i == 1 || $i == $n || $j == 1 || $j == $n) ? "*" : " ";
    }
    echo "\n";
}
```

---

### ✅ 13. Cross (X) Pattern

```php
$n = 5;
for($i = 1; $i <= $n; $i++) {
    for($j = 1; $j <= $n; $j++) {
        echo ($j == $i || $j == $n - $i + 1) ? "*" : " ";
    }
    echo "\n";
}
```

---

### ✅ 14. Numeric Square

```php
for($i = 1; $i <= 5; $i++) {
    echo str_repeat($i, 5) . "\n";
}
```

---

### ✅ 15. Incrementing Number Triangle

```php
$k = 1;
for($i = 1; $i <= 5; $i++) {
    for($j = 1; $j <= $i; $j++) echo $k++ . " ";
    echo "\n";
}
```

---

### ✅ 16. Reverse Number Triangle

```php
for($i = 5; $i >= 1; $i--) {
    for($j = $i; $j >= 1; $j--) echo $j;
    echo "\n";
}
```

---

### ✅ 17. Star with Space Triangle

```php
for($i = 1; $i <= 5; $i++) {
    for($j = 1; $j <= $i; $j++) echo "* ";
    echo "\n";
}
```

---

### ✅ 18. Mirror Number Triangle

```php
for($i = 1; $i <= 5; $i++) {
    echo str_repeat(" ", 5 - $i);
    for($j = 1; $j <= $i; $j++) echo $j;
    echo "\n";
}
```

---

### ✅ 19. Alphabet Triangle

```php
for($i = 65; $i < 70; $i++) {
    for($j = 65; $j <= $i; $j++) echo chr($j);
    echo "\n";
}
```

---

### ✅ 20. Hollow Triangle

```php
$n = 5;
for($i = 1; $i <= $n; $i++) {
    for($j = 1; $j <= $i; $j++) {
        if ($j == 1 || $j == $i || $i == $n) echo "*";
        else echo " ";
    }
    echo "\n";
}
```

---

