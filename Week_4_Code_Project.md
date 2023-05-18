# Week 4 Code Project

### Draw Flag

```python
from graphics import Canvas
import random

CANVAS_WIDTH = 450
CANVAS_HEIGHT = 300

def main():
    canvas = Canvas(CANVAS_WIDTH, CANVAS_HEIGHT)
    # TODO, your code here
    canvas.create_rectangle(0,0,CANVAS_WIDTH,CANVAS_HEIGHT/2,"red")
    canvas.create_rectangle(0,CANVAS_HEIGHT/2,CANVAS_WIDTH,CANVAS_HEIGHT,"white")

if __name__ == '__main__':
    main()
```

### Khansole Academy

```python
import random

def main():
    print("Khansole Academy")
    
    random_integer1 = generate_two_digit_integers()
    random_integer2 = generate_two_digit_integers()
    expect_sum = sum_of_two_numbers(random_integer1,random_integer2)
    
    #Ask the answer of the addition question and get the user's input
    print("What is " + str(random_integer1) + " + " + str(random_integer2) + " ?")
    user_answer = int(input("What is " + str(random_integer1) + " + " + str(random_integer2) + " ?"))
    
    #Check if the answer is correct
    if expect_sum==user_answer:
        print("Correct!")
    else:
        print("Incorrect!")
        print("The expected answer is " + str(expect_sum))

def generate_two_digit_integers():
    return random.randrange(10,99)
    
def sum_of_two_numbers(a,b):
    return a + b

if __name__ == '__main__':
    main()
```

