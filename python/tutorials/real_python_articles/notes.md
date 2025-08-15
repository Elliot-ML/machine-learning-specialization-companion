
# **Variables**
In Python, variables are **references** that refer to objects or values (everything in Python is an object actually) stored in the computer's memory.

I can think of a variable as a **container** for a value or a **binding** or **link** to a value.

Variables make it easy to manipulate and reuse values throughout the code.
In Python, I do not have to declare a variable before initialize it. Like in some programming languages:

    let a; #JavaScript
    int b; #C

Instead I declare and initialize the variable through one line of code that assigns a value to the variable and I do not specify the variable type because Python is a dynamically typed (meaning variable types are determined and checked at runtime rather than during compilation):

    name = "BenX" #str
    age = 400 #int
    favourite_number = 3.1416 #float
    interests = ["machine learning", "stock exchange", "books", "cinema"] #list
    favourite_ones = {
        "book"  : "In Search of Lost Time",
        "game"  : "Sonic & All Stars Racing Transformed",
        "movie" : "The Social Network",
        "number": 3.1416,
        "person": "Alan Turing",
    } #dict

## **Expressions**
In Python, an **expression** is a **simple statement** that Python can evaluate to produce and return a value.

Following expressions compute the circumference of two different circles:

    2 * 3.1416 * 10 #62.912
    2 * 3.1416 * 20 #125.824

or

    3.1416

Each of these expressions represent a specific computation that produce a value.
For each expression I have to repeat the input values (2 * 3.1416 * 10 or 3.1416), which is an error-prone and repetitive task.

Instead I'll assign expressions (10, 20, 3.1416) to variables to build other expressions (2 * 3.1416 * 10 or 2 * pi * radius_1):

    pi = 3.1416
    radius_1 = 10
    radius_2 = 20

    2 * pi * radius_1 #62.912
    2 * pi * radius_2 #125.824

## **Some Use Cases of Variables**

### **Counters**
A **counter** is an _int_ variable that allows me to count objects. Counters typically have an initial value of **zero**, which increments each time a given object appears.

    str_counter = 0

    str_int = ["Kaissu", "BenX", 400, 300, "Horoz", False]

    for item in str_int:
        if isinstance(item, str):
            str_counter += 1
    
    print(str_counter) #3

My counter **str_counter** counts the string objects in **str_int** list.

### **Accumulators**
An **accumulator** is a variable that I use to add consecutive values to form a total. I can also use accumulators as parts of larger computations:

    numbers = [0, 1, 2, 3]
    total = 0

    for number in numbers:
        total += number
    
    print(total) #6

    mean = total / len(numbers) #1.5, an accumulator as a part of a larger computation (mean computation).

Python has built-in functions that act like a counter or an accumulator. **_len()_** function counts the number of objects in a sequence whereas **_sum()_** function sums all the objects in a sequence.

    len(numbers) #4
    sum(numbers) #6



