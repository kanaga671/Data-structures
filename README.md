# Priority Queue using List

pq = []

# Insert element

def enqueue(item, priority):

pq.append((priority, item))

pq.sort(reverse=True) # Higher number = higher priority

# Delete element

def dequeue():

if not pq:

return "Queue is empty"

return pq.pop(0)

# Example

enqueue("Task1", 2)

enqueue("Task2", 5)

enqueue("Task3", 1)

print("Priority Queue:", pq)

print ("Removed:", dequeue())

print("After Deletion:", pq)

Output:

Priority Queue: [(5, 'Task2'), (2, 'Task1'), (1, 'Task3')] Removed: (5, 'Task2') AUTONOMOUS After Deletion: [(2, 'Task1'), (1, 'Task3')]# Data-structures
