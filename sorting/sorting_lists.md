## Sorting Lists


#### The simplist methoed is the sorted(list) function
```
a = [2, 1, 4, 3]
print(sorted(a))  ## [1, 2, 3, 4]
print(a)  ## [2, 1, 4, 3]
```

#### Watch out because sorted() is case sensitive
```
strs = ['G', 'B', 'a', 'c']
print(sorted(strs))  ## ['B', 'G', 'a', 'c'] case sensitive!
print(sorted(strs, reverse=True))   ## ['c', 'a', 'G', 'B']
```

#### Sorting with a key
```
strs = ['aaaaa', 'z', 'ssss', 'bb']
print sorted(strs, key=len)  ## ['z', 'bb', 'ssss', 'aaaaa']
```

#### For case insensitive sorting you can use str.lower as the key
```
strs = ['G', 'B', 'a', 'c']
print sorted(strs, key=str.lower)  ## ['a', 'B', 'c', 'G']
```
