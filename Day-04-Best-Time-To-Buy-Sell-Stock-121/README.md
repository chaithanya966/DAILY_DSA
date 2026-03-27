# Best Time to Buy and Sell Stock (LeetCode #121)

## 🧩 Problem

Given an array `prices` where `prices[i]` is the price of a stock on day i, find the maximum profit you can achieve.

You may choose only one day to buy and one different day to sell.

---

## 💡 Approach (Greedy / Minimum Tracking)

* Keep track of the **minimum price** seen so far
* For each day:

  * Calculate profit = current price - minimum price
  * Update maximum profit
* Update minimum price if a lower price is found

---

## 🚀 Algorithm Steps

1. Initialize `minPrice = Integer.MAX_VALUE`
2. Initialize `maxProfit = 0`
3. Traverse array:

   * Update minPrice
   * Calculate profit
   * Update maxProfit
4. Return maxProfit

---

## ⏱ Time Complexity

O(n)

## 💾 Space Complexity

O(1)

---

## 🧠 Key Learning

* Greedy approach
* Tracking minimum value
* Optimizing brute force O(n²) to O(n)

---

## ✅ Example

Input:
[7,1,5,3,6,4]

Output:
5

Explanation:
Buy at price 1 and sell at price 6 → profit = 5
// fixing contribution issue
// new commit for green dot