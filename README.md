# Multi-Branch Feature Integration & Conflict Resolution Strategy

## Overview
This project demonstrates a multi-contributor Git workflow simulating a team environment. The goal was to build a complete feature by splitting the work across separate contributor branches, aggregating them into an integration branch, resolving initial merge conflicts, and finally merging into `main` while respecting branch protection policies.

---

## Branching Strategy

```text
main (Protected)
  ▲
  │ (Final Pull Request)
  │
feature/combine (Integration Branch)
  ▲                     ▲
  │ (Merge)             │ (Merge)
  │                     │
feature/login1        feature/login2
(Account A)           (Account B)