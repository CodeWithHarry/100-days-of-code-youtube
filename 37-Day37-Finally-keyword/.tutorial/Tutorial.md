# Finally Clause
The finally code block is also a part of exception handling. When we handle exception using the try and except block, we can include a finally block at the end. The finally block is always executed, so it is generally used for doing the concluding tasks like closing file resources or closing database connection or may be ending the program execution with a delightful message.
# Syntax:
```
try:
   #statements which could generate 
   #exception
except:
   #solution of generated exception
finally:
    #block of code which is going to 
    #execute in any situation
    
   
```
The finally block is executed irrespective of the outcome of try……except…..else blocks\
One of the important use cases of finally block is in a function which returns a value.
# Example:
```python
try:
    num = int(input("Enter an integer: "))
except ValueError:
    print("Number entered is not an integer.")
else:
    print("Integer Accepted.")
finally:
    print("This block is always executed.")
 ```

## Output 1:
```
Enter an integer: 19
Integer Accepted.
This block is always executed.
```
## Output 2:
```
Enter an integer: 3.142
Number entered is not an integer.
This block is always executed.
```
## [Next Lesson>>](https://replit.com/@codewithharry/38-Day38-Custom-Errors)