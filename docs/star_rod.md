# Star Rod

Star Rod is a modding tool created by Clover. While Star Rod can be used to create mods on its own, it does not support
writing mods in C, and it does not support adding other mods as dependencies. Merlon, however, leverages the
[Paper Mario decompilation](https://papermar.io) to provide much more powerful modding capabilities.

## Comparison with Star Rod

| Feature                                              | Star Rod | Merlon                 |
| ---------------------------------------------------- | -------- | ---------------------- |
| Open source                                          | No       | Yes                    |
| Mod management                                       | Yes      | Yes                    |
| Supported base ROM versions                          | 🇺🇸       | 🇺🇸                     |
| Distributable format                                 | `.mod`   | `.merlon`              |
| View source code of distributable                    | No       | Yes                    |
| Dependency management                                | No       | Yes                    |
| C language support                                   | No       | Yes (decomp)           |
| `.mpat`/`.bpat` language support                     | Yes      | No                     |
| Compile modded ROM                                   | Yes      | Yes (`merlon build`)   |
| Easily run modded ROM in emulator                    | No (manual) | Yes (`merlon run`)  |
| GUI Map editor                                       | Yes      | No (use Star Rod)      |
| GUI Sprite editor                                    | Yes      | No (use Star Rod)      |
| GUI World editor                                     | Yes      | No                     |
| GUI Image editor                                     | Yes      | No                     |
| CLI-GUI feature parity                               | No       | Yes                    |

## Using the Star Rod editors with Merlon

```{note}
The Star Rod world editor and image editor are **not** compatible with Merlon.
```

Star Rod's map, string (message), and sprite editors can be used with Merlon. To do so:

1. Open Star Rod.
2. Open the *Mod Manager*.
3. Change the *Mod Folder* to the `papermario` subdirectory of your [initialised](getting_started.md#initialisation) Merlon package.
4. _Dump Assets_ if you haven't already.
5. _Copy Assets to Mod_.
6. Close and reopen Star Rod.
7. Open an editor.
