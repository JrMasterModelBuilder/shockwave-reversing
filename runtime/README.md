# Runtime

Shockwave uses Lingo or JavaScript code compiled to a custom format.


## Opcodes

Each opcode is a single byte, where the highest 2 bits indicate how many bytes are need to be decoded any following integer.

```
00 = 0 bytes
01 = 1 bytes
10 = 2 bytes
11 = 4 bytes
```

For this reason many opcode handlers are registered several times.

See `opcodes.txt` for a list of all opcodes and their handler symbol name.
