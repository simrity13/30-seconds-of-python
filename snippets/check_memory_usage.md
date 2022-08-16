---
title: check_memory_usage
tags: string
expertise: intermediate
firstSeen: 2022-08-16T14:00:00:000
---

Check the Memory Usage of an Object

- The standard library's sys module provides the getsizeof() function.
- That function accepts an object (and optional default), calls the object's sizeof() method, and returns the result, so you can make your objects inspectable as well.

```py
def check_memory_usage(data):
    return sys.getsizeof(data)
```

```py
print(check_memory_usage("simrity")) # 56
print(check_memory_usage("dinesh")) # 55
print(check_memory_usage("Hello world")) # 60
```
