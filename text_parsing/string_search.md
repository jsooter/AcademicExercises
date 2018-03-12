## Strings in Strings

The easiest way to find a string within a string (substring) is to use the *in* operator:
```py
mystring = "hello world"

if "world" in mystring:
    print("found")
else:
    print("not found")
```
Here is an example using the *find()* string method:
```py
# using find()
if mystring.find() != -1:
    print("found")
else:
    print("not found")
```
Here is an example using the *index()* method:
```py
# index method:
try:
    mystring.index("world")
except ValueError:
    print("not found")
else:
    print("found")


```
