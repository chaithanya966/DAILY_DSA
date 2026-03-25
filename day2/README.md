# Valid Palindrome (LeetCode #125)

## 🧩 Problem

Given a string `s`, determine if it is a palindrome, considering only alphanumeric characters and ignoring cases.

---

## 💡 Approach (Two Pointer)

* Use two pointers:

  * `left` starting from beginning
  * `right` starting from end
* Skip non-alphanumeric characters using:
  `Character.isLetterOrDigit()`
* Convert characters to lowercase for comparison
* Compare both sides:

  * If mismatch → return false
  * Else → move both pointers inward

---

## 🚀 Algorithm Steps

1. Initialize `left = 0`, `right = s.length() - 1`
2. Loop while `left < right`
3. Skip invalid characters
4. Compare lowercase characters
5. Move pointers inward
6. If all match → return true

---

## ⏱ Time Complexity

O(n)

## 💾 Space Complexity

O(1)

---

## 🧠 Key Learning

* Two Pointer Technique
* String traversal
* Handling edge cases (spaces, symbols, case sensitivity)

---

## ✅ Example

Input:
"A man, a plan, a canal: Panama"

Output:
true

Explanation:
After removing special characters:
"amanaplanacanalpanama"
which is a palindrome.
