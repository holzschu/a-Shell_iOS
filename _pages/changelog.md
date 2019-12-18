---
layout: page
title: What's New
include_in_header: true
---

# Changelog

<br>

### `Latest`
# **Version 1.3**
#### What's New
- the cursor is now indicating the active window 
- we've added the [taskwarrior](https://taskwarrior.org) utilities (`task`) 
- we've added the `clang` and `clang++` compilers. They translate your C code into LLVM bytecode (IR), which you can execute using the LLVM interpreter (`lli`).
```
$ clang file.c
$ lli file.ll
```
- you can even combine multiple bytecode files together with `llvm-link`:
```
$ clang file1.c
$ clang file2.c
$ llvm-link -o result.bc file1.ll file2.ll
$ lli result.bc
```
- Your programs have access to the C library, so `printf()`, `scanf()`, etc... work.
- C++ input/output functions do not work. Its main use is to check for syntax errors in your code.
- You can also compile to WebAssembly or Arm64 targets, but not execute the result of your compilations. 


#### Bug fixes
- fixed the Python installation (this removes the `No module named "encodings"` error)
- more robust job management in Vim

<br>

# **Version 1.2**

#### What's New
- a-Shell now saves your session content as soon as you go in the background, and restores it when the app goes in the foreground, even if it was terminated by iOS. 
- specifically, we save and restore, for all windows: the content of the buffer, the command history and the command that is running.
- if Vim is running, we also save all opened files. We restore the content and position of all buffers and tabs, using [vim-session](https://github.com/xolox/vim-session).
- permissions to access distant files and folders is also saved for future use. 
- you can list existing permissions with "bookmarks", open a specific distant file or folder with "jump", rename bookmarks with "renamemark".
- a-Shell automatically creates a bookmark every time you open a distant file or folder (e.g. with "pickFolder") but you can rename it later.
- you can remap caps-lock to escape, which can be useful for Vim users. As a side effect, this enables auto-repeat on external keyboards. 
- Vim was updated to the latest minor version. 

#### Bug Fixes
- accented characters had issues on some keyboards (not all). This is fixed now.

<br>

________
<br>

# **Version 1.1**

#### What's New
Opening files in Vim when Vim is already running: you have the option to open in new Window (default), new tab or new buffer. 

#### Bug Fixes
- a-Shell can now open files with spaces in their names. That includes files from iCloud and external file providers. 

<br>

# **Version 1.0**
First release on the AppStore. 

<br>
