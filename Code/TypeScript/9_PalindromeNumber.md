# LeetCode Problem #9 — Palindrome Number

## Problem Description
Given any Real Number, check if it is a palindrome.

---

## Solution (TypeScript)

```typescript

function isPalindrome(x: number): boolean {

    const num = x;

    if (x < 0) return false;
    let ans = 0;

    while (x > 0) {
        const r = x % 10;
        ans = ans * 10 + r;
        x = Math.floor(x / 10);
    }

    return num == ans;
    
};
