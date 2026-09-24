# 🔍 Contains Duplicate

This project contains my Python solution for the **Contains Duplicate** problem from LeetCode.

## 🧩 Problem

Given an integer array `nums`, return `True` if any value appears at least twice.

Return `False` if every element in the array is unique.

## 💡 Example

### Input

```text
[1, 2, 3, 1]
```

### Output

```text
True
```

### Explanation

The number `1` appears twice in the array.

## 🐍 Python Solution

```python
class Solution:
    def containsDuplicate(self, nums):
        seen = set()

        for num in nums:
            if num in seen:
                return True

            seen.add(num)

        return False


solution = Solution()

nums = [1, 2, 3, 1]

print(solution.containsDuplicate(nums))
```

### Output

```text
True
```

## 🔍 Approach

We use a Python `set` called `seen` to store numbers that we have already visited.

For every number:

1. Check whether the number is already in `seen`.
2. If it is, a duplicate exists, so return `True`.
3. Otherwise, add the number to `seen`.
4. If we finish the loop without finding a duplicate, return `False`.

This uses a hash set and checks the array in one pass.

## ⏱️ Complexity

* **Time Complexity:** `O(n)`
* **Space Complexity:** `O(n)`

## 🛠️ Technologies

* Python
* LeetCode
* VS Code
* Git & GitHub

## ▶️ How to Run

1. Open the project in VS Code.
2. Open the Python file.
3. Save the file using `Ctrl + S`.
4. Open the VS Code terminal.
5. Run:

```bash
python filename.py
```

## 📚 What I Learned

* How to use Python `set`
* How to detect duplicate values
* Using `for` loops
* Understanding hash-based searching
* Understanding `O(n)` time complexity
* Solving LeetCode problems using Python
* Using Git and GitHub

## 🚀 Learning Journey

This project is part of my **LeetCode problem-solving journey**.

I am practicing Python, Data Structures, Algorithms, and problem-solving skills one problem at a time.

---

⭐ **Keep learning and keep coding!**
