---
layout: post
title: 'Python 101: The Absolute Minimum You Need to Know'
date: 2025-06-20 23:45 -0700
tags: python, programming, beginner, coding, tutorial
---

> “If you understand this banana, you understand Python.”

Learning Python can feel overwhelming — variables, loops, functions, classes... it's **a lot**. Of course, to truly master Python, you need to understand all these concepts in depth. But in 2025, we learn by **building** things, not walking through the definitions one by one. 

So, let’s start with the **absolute minimum** you need to know to get going with Python, using a simple example: a banana. 🍌

---

## Banana 🍌

Let’s code up a `banana` in Python.  
This banana will **age** over time, and **change color** depending on how many days have passed.

```python
class Banana:
    def __init__(self):
        self.days = 0

    def age(self, days):
        for _ in range(days):
            self.days += 1

        if self.days > 10:
            color = "brown"
        else:
            color = "yellow"

        print(f"This banana is now {color}")

banana = Banana()
banana.age(14)
```

You just used the fundamentals of Python, all at once! Let's peel back the layers one-by-one (pun intended), and see what’s going on here. 🥳

#### 1. Variables
```python
self.days = 0
color = "yellow"
```
Variables are used to store data. Simple as that.

#### 2. Functions
```python
def age(self, days):
    ...
```
Functions are reusable blocks of code. They take input (days) and do something with it.

#### 3. Loops
```python
for _ in range(days):
    self.days += 1
```
This for loop runs once for each day passed, adding 1 to the banana’s age.

#### 4. Conditionals (if/else)
```python
if self.days > 10:
    color = "brown"
else:
    color = "yellow"
```
This is decision-making: we check how old the banana is and assign a color accordingly.

#### 5. Classes and Objects
```python
class Banana:
    ...
```

You defined a class — a blueprint for bananas.

Then you made a real banana:

```python
banana = Banana()
banana.age(14)
```

And you ran the method on that object. Boom.

#### Output
```bash
➜ python banana.py
This banana is now brown
```

Why? Because 14 days have passed, and the banana turned brown. 🍌💀

---

You just learnt 5 key concepts in Python from 14 lines of code. In fact, these concepts are the **building blocks** of almost every Python program you'll write.
You can now create more complex programs by combining these concepts.

Want to play around? Here's the [collab notebook](https://colab.research.google.com/drive/1FA6jzmb6mXXl8HFbczuxzaWljhD9iNoY?usp=sharing) to run this code.

## What’s Next?

Next step is to continue learning a few more basics. We will try building a fridge to learn concepts like dictionaries, lists, and more complex logic.


If this helped, share it with a friend learning to code.

Happy coding! 🚀
