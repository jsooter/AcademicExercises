## Directory Functions

See [os.path](https://docs.python.org/3/library/os.path.html) for reference to file system path funtions.

Check to see whether a certain file path is a directory

```py
import os

if os.path.isdir("/tmp"):
    print("/tmp is a directory"
else:
    print("/tmp is not a directory")
```
