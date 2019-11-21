---
layout: page
title: What's New
include_in_header: true
---

# Changelog

<br>

### `Latest`
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

# **Version 1.1**

#### What's New
Opening files in Vim when Vim is already running: you have the option to open in new Window (default), new tab or new buffer. 

#### Bug Fixes
- a-Shell can now open files with spaces in their names. That includes files from iCloud and external file providers. 

# **Version 1.0**
First release on the AppStore. 

<br>
