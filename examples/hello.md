Hello World
---

`mdscript` is a mini tool to exectue codes inside the markdown file in a flexiable way. Here are some examples of the Hello World program.

To see the output, run `mdscript hello.md` in your terminal.

A python example

```python, @mdscript
print("Hello World!")
```

A javascript example

```javascript, @mdscript
console.log("Hello World!")
```

A C example

```c, @mdscript
#include <stdio.h>

int main() {
    printf("Hello World!");
    return 0;
}
```

Remove the code block

```c, @mdscript(--no-code)
#include <stdio.h>

int main() {
    printf("Hello World!");
    return 0;
}
```
