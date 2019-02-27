# iKernel
iKernel is a module to run python code inside python comments!
```python
from ikernel import auto_exec;
'''
<?
i : int;
for i in range(10):
    print(i);
?>
'''
f = auto_exec();
```
Output:
```python
0
1
2
3
4
5
6
7
8
9
```
Another example:
```python
from ikernel import auto_exec;
'''
<?
b : list = [1, 3, 5, 6];
i : int;
for i in range(len(b)):
    if (b[i] == 6):
        print("A six was found");
?>
'''
f = auto_exec();
```
Output:
```python
A six was found
```
