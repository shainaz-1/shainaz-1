- 👋 Hi, I’m @shainaz-1
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
shainaz-1/shainaz-1 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

v

import heapq

class PriorityQueue:
    def __init__(self):
        self._queue = []
        self._index = 0  # To handle elements with the same priority

    def push(self, item, priority):
        """Add an item to the priority queue with given priority."""
        heapq.heappush(self._queue, (priority, self._index, item))
        self._index += 1

    def pop(self):
        """Remove and return the item with the highest priority."""
        if self.is_empty():
            raise IndexError("pop from empty priority queue")
        return heapq.heappop(self._queue)
if __name__ == "__main__":
    pq = PriorityQueue()

# Check if the priority queue is empty
    print("Is empty:", pq.is_empty())  # Output: Is empty: False

import heapq

class PriorityQueue:
    def __init__(self):
        self._queue = []
        self._index = 0  # To handle elements with the same priority

    def push(self, item, priority):
        """Add an item to the priority queue with given priority."""
        heapq.heappush(self._queue, (priority, self._index, item))
        self._index += 1

    def pop(self):
        """Remove and return the item with the highest priority."""
        if self.is_empty():
            raise IndexError("pop from empty priority queue")
        return heapq.heappop(self._queue)
if __name__ == "__main__":
    pq = PriorityQueue()

# Check if the priority queue is empty
    print("Is empty:", pq.is_empty())  # Output: Is empty: False
