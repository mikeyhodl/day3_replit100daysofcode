# Common Coding Errors

*Copy each of the code blocks below with 👉 to `main.py`, click run, and see if you can fix them!
Make sure to get rid of any old code from `main.py` before you start the next one.*

## Invalid Syntax

👉 Copy the code below, hit `run` and see what happens.

```python
yourName = input("Name: ")
whatYear = input("What year is it?: ")
print(yourName "thinks it is" whatYear)
```
What does this error mean? How can you fix it?
```
  File "main.py", line 3
    print(yourname "thinks it is" whatYear)
                   ^
SyntaxError: invalid syntax
 
```


<details><summary>Answer 👀</summary>
  
- An easy mistake to make is to forget one or more commas.
- Remember that you need a `,` ***between*** each different object you're trying to print out.
- Without `,` the computer gets confused and shows an error.
</details>

## Your code may run...but look weird
👉 This code would *actually run*, but...



```python
yourName = input("Name: ")
whatYear = input("What year is it?: ")
print("yourName, thinks it is, whatYear")
```
give this output. What's weird about this code?
```
Name: Mark
What year is it?: 2431
yourname, thinks it is, whatYear
```
<details><summary>Answer 👀</summary>

  - Another common error occurs when you wrap the entire thing in **quotes** `(".., .., .. ")`.
  - This *actually runs*, but doesn't quite do what you want.
  - Everything in `(".., .., .. ")` gets printed *literally*.
  - Since the variable names are alo within quotes `(".., .., .. ")`, it's literally printing the names rather than the contents.
    - The only thing in quotes should be the *literal* strings `print(varName, "literal string", varName2)`.
</details>

