# sudo-win

A utility for running arbitrary command with administrator access on Windows

**Use the following command to compile:**

```sh
  gcc -std=c99 -Wall -Wextra -Werror -Wconversion -pedantic -pedantic-errors \
    sudo.c -o sudo.exe -O3 -nostdlib -lshlwapi -lshell32 -lkernel32 \
    -Wl,--entry,@SudoEntryPoint,--subsystem,windows,--strip-all
```
