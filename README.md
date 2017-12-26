# glock
A cross-platform, globally, named lock for Python.

# Simple usage

```
pip install glock
```

test.py
```python
import time
import os
from glock import Glock


print("{} acquiring lock".format(os.getpid()))

whih GLock(name="a_global_name"):
    print("{} acquired lock".format(os.getpid()))
    time.sleep(10)
```

bash1:

```bash
python test.py
```

bash2:

```bash
python test.py
```
