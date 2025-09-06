

# **Experiment-13** :  **Pytest – Python program for Sum of Digits**


## **Aim:**

To write a Python program using **Pytest** for testing the sum of digits of a number.

---

## **Algorithm:**

1. Start the program.
2. Write a Python function `sum_of_digits(n)` that calculates the sum of digits of a number.
3. Create a separate test file named **test\_sumofdig.py**.
4. Inside it, write test functions with `assert` statements for different cases.
5. Run the tests using the command:

   ```bash
   pytest -s TEST_EX13.py
   ```
6. If all assertions pass, the function is correct.

---

## **Program:**

**EX13.py**

```python
def sum_of_digits(n):
    total = 0
    while n > 0:
        total += n % 10
        n //= 10
    return total
```

**TEST_EX13.py**

```python
from EX13 import sum_of_digits

def test_sum_of_digits():
    print()

    print("sum_of_digits(123) =", sum_of_digits(123))  
    assert sum_of_digits(123) == 6

    print("sum_of_digits(4567) =", sum_of_digits(4567))
    assert sum_of_digits(4567) == 22

    print("sum_of_digits(0) =", sum_of_digits(0))      
    assert sum_of_digits(0) == 0

    print("sum_of_digits(9999) =", sum_of_digits(9999)) 
    assert sum_of_digits(9999) == 36
```

---

## **Output:**

## **Result:**

Thus, the Pytest program for Sum of Digits (EX13.py & TEST_EX13.py) was successfully written, executed, and tested. ✅

