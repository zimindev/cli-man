# 📘 man — Manual Pages for Unix/Linux Commands

The `man` command shows the manual (documentation) for other terminal commands, programs, system calls, and configuration files. It’s the first place you should check when learning or troubleshooting a command.

---

## ✅ Features

- Provides in-depth documentation for almost all Linux/Unix tools
- Structured into sections (commands, libraries, config files, etc.)
- Searchable and easy to navigate
- Works offline

---

## 🔧 Syntax

```bash
man [section] command
```

- `section` (optional): Manual section number (1–9)
- `command`: The name of the command or topic

---

## 📂 Manual Sections

| Section | Description                  |
|---------|------------------------------|
| 1       | User commands                |
| 2       | System calls                 |
| 3       | C library functions          |
| 4       | Special files (e.g. /dev)   |
| 5       | File formats and configs     |
| 6       | Games and screensavers       |
| 7       | Miscellaneous info           |
| 8       | System admin commands        |
| 9       | Kernel routines (rare)       |

Example:
```bash
man 5 passwd
```
> Shows the man page for the `passwd` file format, not the command.

---

## 🚀 Usage Examples

### View a manual page
```bash
man ls
```

### Search for a keyword
```bash
man -k zip
```
> Lists all man pages with “zip” in their name or description.

### Open specific section
```bash
man 5 crontab
```

### Show man page path
```bash
man -w ls
```

---

## ⌨️ Keyboard Navigation

| Key        | Action                         |
|------------|--------------------------------|
| `Arrow Up/Down` | Scroll line-by-line       |
| `Page Up/Page Down` | Scroll by page       |
| `q`         | Quit man page                 |
| `/pattern`  | Search for a pattern forward  |
| `n`         | Next search result            |
| `N`         | Previous search result        |

---

## 🔄 Related Commands

| Command     | Description                            |
|-------------|----------------------------------------|
| `whatis`    | One-line description of a command      |
| `apropos`   | Search man pages by keyword            |
| `info`      | GNU-style documentation (more verbose) |
| `--help`    | Quick help for many commands           |

---

## 📚 More Info

- Manual of man:
```bash
man man
```

- Official man-db project: [https://savannah.nongnu.org/projects/man-db](https://savannah.nongnu.org/projects/man-db)

---

## 🧩 Tips

- If `man` pages appear as raw code or are missing, install the relevant `man` packages, e.g.:
```bash
sudo apt install man-db manpages
```

- Use `man -k .` to list all available man pages.

- Some distributions split man pages into multiple packages (e.g., `manpages-dev` on Debian).
