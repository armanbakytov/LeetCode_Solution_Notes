# LeetCode Solution Notes

Decided to restart my LeetCode journey and actually **understand** things this time, not just pass the judge and forget the logic 10 minutes later :)

This repo is my scratchpad of solutions, thoughts, mistakes, and small insights while solving LeetCode problems.

I linked this repo to my Obsidian Vault and will try to document my solutions whenever I have free time.

---

## What’s inside

Each problem lives in its own markdown file:

- `1. Two Sum.md`
- `2. Add Two Numbers.md`
- `3. Longest Substring Without Repeating Characters.md`
- ...

The idea is not to collect perfect solutions, but to document:

- what the problem is asking,
- how I *first* tried to solve it (even if it’s dumb or O(n²)),
- how I improved it,
- what pattern it belongs to.

---

## File structure / my note style

Most files roughly will follow this structure:

### 1. Problem Description

Short restatement of the problem in my own words, plus the key constraints.

Example:

> We’re given two linked lists that represent numbers in **reverse** order.  
> Each node is a digit. Add them like in high school and return the result as a linked list.

If the statement has any trick (like “substring vs subsequence”, “reverse order”, etc.), I highlight that.

---

### 2. Solution Process

This is where I think out loud:

- First ideas, even if they’re not optimal.
- What I *wanted* to do.
- Where it breaks (like failing on `"abba"` or edge cases).

Example style:

> We have a singly linked list, so no going back.  
> It’s literally just school addition: sum digits, keep carry, move on.  
> Treat null nodes as `0` once one list ends.

Sometimes I’ll write small pseudo-code blocks:

```pseudocode
sum = node1 + node2 + carry
digit = sum % 10
carry = sum / 10
append digit as new node
```
