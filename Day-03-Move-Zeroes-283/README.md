# Move Zeroes (LeetCode #283)

## 🧩 Problem

Move all zeros to the end of the array while maintaining the relative order of non-zero elements.

---

## 💡 Approach (Two Pointer)

* Use two pointers:

  * `i` → scans array
  * `j` → position for next non-zero
* When non-zero found:

  * Swap with `j`
  * Increment `j`

---

## ⏱ Time Complexity

O(n)

## 💾 Space Complexity

O(1)

---

## 🧠 Key Learning

* Two pointer (same direction)
* In-place array manipulation
