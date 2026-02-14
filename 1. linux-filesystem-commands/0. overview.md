# Linux Command Reference Guide

A comprehensive guide to essential Linux terminal commands for navigating the filesystem, managing files, and building projects.

---

## Commands

### Navigation
- [pwd](pwd.md) - Print Working Directory
- [ls](ls.md) - List Directory Contents
- [cd](cd.md) - Change Directory
- [tree](tree.md) - Display Directory Tree Structure

### File Viewing
- [cat](cat.md) - Concatenate & Display Files
- [head & tail](head-tail.md) - View File Beginnings and Endings
- [more & less](more-less.md) - File Pagers for Scrolling

### File Management
- [touch](touch.md) - Create Files & Modify Timestamps
- [mv](mv.md) - Move and Rename Files
- [rm](rm.md) - Remove Files & Directories
- [echo](echo.md) - Print Text & Write to Files

### Directory Management
- [mkdir](mkdir.md) - Make Directory
- [rmdir](rmdir.md) - Remove Empty Directories

### Editors & Tools
- [nano](nano.md) - Terminal Text Editor
- [make](make.md) - Build Automation Tool

---

## Quick Reference Card

| Command | Purpose | Most Used Flags |
|---------|---------|-----------------|
| `pwd` | Print current directory | `-P` (physical path) |
| `ls` | List directory contents | `-la`, `-lh`, `-lt` |
| `cd` | Change directory | `-`, `..`, `~` |
| `tree` | Display directory tree | `-L`, `-a`, `-d` |
| `cat` | Display/combine files | `-n`, `-s`, `-A` |
| `head` | View file beginning | `-n`, `-c` |
| `tail` | View file end / follow | `-n`, `-f`, `-F` |
| `more` | Simple file pager | `+/pattern`, `-d` |
| `less` | Advanced file pager | `-N`, `-S`, `-R`, `+F` |
| `touch` | Create files/update timestamps | `-d`, `-r`, `-c` |
| `mv` | Move/rename files | `-i`, `-n`, `-v`, `-b` |
| `rm` | Remove files/directories | `-r`, `-f`, `-i` |
| `mkdir` | Create directories | `-p`, `-v` |
| `rmdir` | Remove empty directories | `-p`, `-v` |
| `nano` | Edit text files | `-l`, `-B`, `-m` |
| `echo` | Print text/write files | `-n`, `-e` |
| `make` | Build automation | `-j`, `-n`, `-f` |

---

## File Extensions Reference

In Linux, file extensions are mostly for human convenience. The system uses **File Signatures (Magic Bytes)** to identify file types.

### Extensions by Tool

| Tool | Common Extensions | Primary Purpose |
|------|-------------------|-----------------|
| `touch` | `.txt`, `.log`, `.sh`, `.md` | Create empty files / Update timestamps |
| `nano` | `.conf`, `.py`, `.c`, `.sh`, `.txt` | Edit text content |
| `echo` | `.txt`, `.sh`, `.env`, `.conf` | Write short strings to files |
| `cat` | `.log`, `.txt`, `.json`, `.csv` | Display or merge content |
| `make` | `Makefile`, `.c`, `.o`, `.h` | Automate builds and compilation |

### Common Extension Categories

#### Documents & Text
- `.txt` - Plain text
- `.md` - Markdown
- `.log` - Log files
- `.csv` - Comma-separated values
- `.json` - JSON data
- `.yaml` / `.yml` - YAML configuration

#### Scripts & Source Code
- `.sh` - Bash/Shell scripts
- `.py` - Python
- `.c` / `.h` - C source/headers
- `.cpp` / `.hpp` - C++ source/headers
- `.js` - JavaScript
- `.rb` - Ruby
- `.pl` - Perl

#### Configuration
- `.conf` - Generic configuration
- `.ini` - INI format
- `.cfg` - Configuration
- `.env` - Environment variables
- No extension - Many config files (`.bashrc`, `hosts`)

#### Build & Compiled
- `Makefile` - Make instructions
- `.o` - Object files (compiled)
- `.so` - Shared libraries
- `.a` - Static libraries
- No extension - Executables in Linux

> **Pro Tip:** Use the `file` command to identify what a file actually is, regardless of its extension:
> ```bash
> $ file mysterious_file
> mysterious_file: PNG image data, 800 x 600, 8-bit/color RGB
> ```
