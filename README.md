[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/KuuIFSwK)
# Weekly Coding #3 — Metro City Help Center

## Summary
This homework uses one connected story to practice stack and queue behavior in Python.

Metro City Help Center needs a small support system for recent staff actions, waiting citizens, request-note checks, and service-line processing.

## How to run
```bash
pytest -q
```

## Complexity
### `ActionStack.pop`
- Time:O(1)
- Why:Removing the last element from a Python list using .pop() takes constant time.

### `RequestQueue.dequeue`
- Time:O(1)
- Why:collections.deque.popleft() removes from the front efficiently in constant time.

### `is_note_balanced`
- Time:O(n)
- Why:The function loops through each character in the string once, and each stack operation (push/pop) is O(1).

### `process_request_line`
- Time:O(n)
- Why:Each citizen is added to the queue once and removed once, so total operations are proportional to the number of citizens.

## Edge-case checklist
- [x] empty action stack
- [x] empty request queue
- [x] empty string for `is_note_balanced`
- [x] note with no brackets
- [x] empty citizen list

## Assistance & sources
- AI used? (Y/N):Y
- What it helped with:Understanding stack and queue implementation, writing functions, and explaining time complexity in a simple way.
- Other sources:Class notes and lecture examples
