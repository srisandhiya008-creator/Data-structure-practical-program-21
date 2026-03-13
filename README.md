# Stack using list
stack = []

# Push (visit a page)
def push(page):
    stack.append(page)
    print(page, "visited")

# Pop (go back)
def pop():
    if len(stack) == 0:
        print("No pages to go back")
    else:
        print(stack.pop(), "removed from stack")

# Display current page
def display():
    if stack:
        print("Current Page:", stack[-1])
    else:
        print("Stack is empty")

# Example
push("Google")
push("YouTube")
push("Wikipedia")

display()

pop()
display()# Data-structure-practical-program-21
