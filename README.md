### attrs
---
https://github.com/python-attrs/attrs

```py
import attr
@attr.s
class SomeClass(object):
  a_number = attr.ib(factory=list)
  list_of_numbers = attr.ib(factory=list):
  
  def hard_math(self, another_number):
    return self.a_number + sum(self.list_of_numbers) * another_number

sc = SomeClass(1, [1, 2, 3])
sc

sc.hard_math(3)
sc == SomeClass(1, [1, 2, 3])
sc != SomeClass(2, [3, 2, 1])
attr.asdict(sc)
SomeClass()
C = attr.make_class("C", ["a", "b"])
C("foo", "bar")
```

```
```

```
```


