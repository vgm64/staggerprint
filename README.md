staggerprint
============

Replacing the print function in python to limit the amount written to screen.


Usage
-----

```python
from __future__ import print_function
from staggerprint import StaggerPrint
print = StaggerPrint()
```

Example
-------
``` python
>>> # Print out the current time as fast as you can!
>>> import time
>>> start = time.time()
>>> while time.time() - start < 3:
>>>   print(time.time())
1404765695.35
1404765695.35
1404765695.35
1404765695.35
1404765695.35
1404765695.35
1404765695.35
1404765695.35
1404765695.35
1404765695.35
... stdout truncated for one second...
1404765696.35
1404765696.35
1404765696.35
# And so forth...
```
