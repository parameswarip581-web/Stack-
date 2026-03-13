# Stack-
Practice program 
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
class Stack:
    def __init__(self):
        self.top = None  # top of stack
    def push(self, data):
        new_node = Node(data)
        new_node.next = self.top
        self.top = new_node
        print "Pushed:", data
    def pop(self):
        if self.top is None:
            print "Stack Underflow"
            return None
        popped_data = self.top.data
        self.top = self.top.next
        print "Popped:", popped_data
        return popped_data
    def peek(self):
        if self.top is None:
            print "Stack is empty"
            return None
print "Top element:", self.top.data
        return self.top.data
    def display(self):
        if self.top is None:
            print "Stack is empty"
            return
        current = self.top
        print "Stack elements:"
        while current:
            print current.data
            current = current.next
stack = Stack()
stack.push(10)
stack.push(20)
stack.push(30)
stack.display()
stack.peek()
stack.pop()
stack.display()
Output:
Pushed: 10
Pushed: 20
Pushed: 30
Stack elements:
30
20
10
Top element: 30
Popped: 30
Stack elements:
20
10
