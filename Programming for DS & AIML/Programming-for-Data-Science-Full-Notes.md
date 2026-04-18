# Programming for Data Science - Complete Notes

---

# 🔹 Unit 1: Python Fundamentals

## Variables & Data Types

* Dynamic typing (no need to declare type)
* Types:

  * int, float, complex

## Scope

* Local → inside function
* Global → entire program

## Example:

```python
total = 100
def func():
    score = 50
    print(score)
func()
print(total)
```

---

## Control Structures (FizzBuzz)

```python
for i in range(1, 21):
    if i % 3 == 0 and i % 5 == 0:
        print("FizzBuzz")
    elif i % 3 == 0:
        print("Fizz")
    elif i % 5 == 0:
        print("Buzz")
    else:
        print(i)
```

---

## File Handling

Modes:

* 'r' → read
* 'w' → write
* 'a' → append

```python
f = open("test.txt", "w")
f.write("Hello")
f.close()
```

---

## Functions & Recursion

```python
def fact(n):
    if n == 1:
        return 1
    return n * fact(n-1)
```

---

## OOP Concepts

* Class & Object
* Inheritance
* Encapsulation
* Polymorphism

```python
class Animal:
    def speak(self):
        print("Animal")

class Dog(Animal):
    def speak(self):
        print("Dog")

d = Dog()
d.speak()
```

---

# 🔹 Unit 2: NumPy & Pandas

## NumPy

```python
import numpy as np
a = np.array([10,20,30])
b = a.reshape(1,3)
```

### Features:

* Fast computation
* Efficient memory

---

## Broadcasting

```python
a = np.array([1,2,3])
print(a * 10)
```

---

## Pandas

### Series & DataFrame

```python
import pandas as pd
s = pd.Series([1,2,3])
df = pd.DataFrame({'A':[1,2]})
```

---

## Missing Values

```python
df.fillna(0)
df.dropna()
```

---

## Merge & Join

```python
pd.merge(df1, df2, on='id')
```

---

## Groupby

```python
df.groupby('Dept').mean()
```

---

# 🔹 Unit 3: Data Visualization

## Plot Types

* Histogram
* Boxplot
* Scatter Plot

```python
import matplotlib.pyplot as plt
plt.scatter([1,2,3],[10,20,30])
plt.show()
```

---

## KDE Plot

```python
import seaborn as sns
sns.kdeplot(data)
```

---

## Matplotlib Architecture

* Figure
* Axes
* Canvas

---

# 🔹 Unit 4: Machine Learning & NLP

## ML Workflow

1. Data collection
2. Preprocessing
3. Training
4. Validation
5. Prediction

---

## Linear Regression

```python
from sklearn.linear_model import LinearRegression
model = LinearRegression()
model.fit(X, y)
```

---

## SVM

```python
from sklearn import svm
model = svm.SVC()
model.fit(X,y)
```

---

## Naive Bayes

```python
from sklearn.naive_bayes import GaussianNB
model = GaussianNB()
```

---

## Feature Engineering

* Scaling
* Encoding
* Handling missing data

---

## NLP Pipeline

* Tokenization
* Stemming
* Lemmatization

```python
from nltk.tokenize import word_tokenize
```

---

# 🔹 Important Short Questions

## = vs ==

* = → assignment
* == → comparison

## Mutable vs Immutable

* List → mutable
* Tuple → immutable

## Lambda Function

```python
square = lambda x: x*x
```

---

## List vs Tuple

| Feature | List | Tuple |
| ------- | ---- | ----- |
| Mutable | Yes  | No    |
| Speed   | Slow | Fast  |

---

## NumPy

* Fast array processing

## Broadcasting

* Different shapes operations

---

## Pandas

* Series (1D)
* DataFrame (2D)

---

## Visualization

* Histogram → distribution
* Scatter → relation

---

## ML Concepts

* Overfitting
* Train-test split
* Cross-validation

---

## NLP

* Stop words
* Bag of Words

---

# 🔥 Summary

* Python basics → foundation
* NumPy & Pandas → data handling
* Visualization → insights
* ML & NLP → intelligence

---
