
# Some Basics of Assembbly Language Writeups

This is the Format to be used to solve all levels 

```python
import pwn
pwn.context.update(arch="amd64")
code = pwn.asm("""

// Enter Your Assembly Here

""")
process = pwn.process("/challenge/embryoasm")
process.write(code)
print(process.readall())
```