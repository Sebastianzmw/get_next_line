# get_next_line

A C function that returns one line at a time from a file descriptor, written at 42 Kuala Lumpur (2024).

```c
char *get_next_line(int fd);
```

- Reads in chunks of `BUFFER_SIZE` bytes and keeps leftover data between calls in a static buffer
- Works with any buffer size, from 1 byte to very large
- **Bonus:** reads from several file descriptors at once without mixing their data

## Use
```sh
cc -Wall -Wextra -Werror -D BUFFER_SIZE=42 get_next_line.c get_next_line_utils.c main.c
```
