# Ashir Ul Haq

# Lab 4 Answers

Chosen topics: Data Structures and Pseudocode.

## Data Structures

### 1. Robot navigating a maze

**Answer:** Stack

**Justification:** A stack removes the last item added first. The robot needs to go back to the last intersection it visited, so a stack works well.

### 2. Processing video packets

**Answer:** Queue

**Justification:** A queue handles the first item added first. This keeps the packets in the order they arrived, so the video plays in the right order.

### 3. Reading sensor temperatures

**Answer:** Array

**Justification:** Each sensor ID can be its position in the array. For example, sensor 25's temperature goes in position 25. The system can go straight to that position to read or change the temperature.

### 4. Checking parentheses, brackets, and braces

**Answer:** Stack

**Justification:** The last symbol opened must be closed first. A stack keeps track of the opening symbols. Each closing symbol must match the opening symbol on top of the stack, which is then removed. If they do not match, the stack is empty when a closing symbol appears, or opening symbols are left at the end, there is an error.

## Pseudocode

### 1. Nested loops

**Answer:** N(N + 1) / 2 calls.

**Justification:** The inner loop runs N times in the first round, N - 1 times in the next round, and one fewer time each round after that. The last round runs once. Adding them gives:

```text
N + (N - 1) + ... + 1 = N(N + 1) / 2
```

### 2. Halving loop with N = 16

**Answer:** 31 calls.

**Justification:** The loop starts at 16 and cuts i in half each round. This means do_work() runs 16, 8, 4, 2, and 1 times. Then i becomes 0 and the loop stops. Adding them gives:

```text
16 + 8 + 4 + 2 + 1 = 31
```
