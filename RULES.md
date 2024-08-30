### Programming Languages

Lower numbered rulesets take precedence. Their suggestions should be taken as requirements. If inapplicable, they are not considered.

- Python
  1. https://peps.python.org/pep-0008/
  2. https://www.kernel.org/doc/html/latest/process/coding-style.html
  3. AussieSeaweed Style
- C/C++
  1. https://www.stroustrup.com/Programming/PPP-style.pdf
  2. https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines#S-functions
  4. https://www.kernel.org/doc/html/latest/process/coding-style.html
  3. https://peps.python.org/pep-0008/
  6. AussieSeaweed Style

### AussieSeaweed Style

1. Group adjacent statements of identical types together.

```Python
assert ...
assert ...
assert ...

x = ...
y = ...

x.foo()
y.zoo()

z = x.evaluate()
w = z + 1

assert ...
return 1
```

2. Trailing commas, even for last item in a list-like context.

```Python
def foo(
    really_long_argument_name: int,
    really_verbose_argument_name: str,
    *,
    really_optional_argument_name: str = 3,
):
    ...

a = [
    'alpha',
    'beta',
    'gamma',
    'theta',
    'zeta',
    'octa',
    'alpha',
    'beta',
    'gamma',
    'theta',
    'zeta',
    'octa',
    'alpha',
    'beta',
    'gamma',
    'theta',
    'zeta',
    'octa',
]
```

3. Commit to breaking lines fully, when done. Enclose by ``()``, ``[]``, etc. if not done already. When breaking, a delimiter should be sent over to the next line.

```
(
    this
    .is()
    .a()
    .really()
    .long()
    .chain()
    .of()
    .method()
    .calls()
)

variable_name = (
    this
    .is()
    .a()
    .really()
    .long()
    .chain()
    .of()
    .method()
    .calls()
)

variable_name = (
    this
    + that
    + and_this
    + plus
    + that
    + again
    + and_again
)

string = (
    'To be or not to be. That is the question.'
    ' Lorem ipsum, blah blah.'
)
```

4. Except in special cases (entrypoint function, etc.), keep function length short (i.e. below 15 lines).
5. never copy paste (no copy-paste programming)
