# 🧩 Contains Duplicate (LeetCode 217)

## 📌 Problem
Given an integer array `nums`, return `true` if any value appears at least twice in the array, and return `false` if every element is distinct.

---

## 🧠 Approach
- Use a HashSet to store elements
- Traverse the array:
  - If element already exists → return true
  - Else → add to set

---

## 🚀 Solution (Java)

```java
import java.util.HashSet;

class Solution {
    public boolean containsDuplicate(int[] nums) {
        HashSet<Integer> set = new HashSet<>();
        
        for (int num : nums) {
            if (set.contains(num)) {
                return true;
            }
            set.add(num);
        }
        
        return false;
    }
}
// day 5 final check