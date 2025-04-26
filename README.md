# ForkEdit
A fast fork/undo for terminal addicts

## fedit + fundo

Simple, Unix-friendly file forking and undo utilities for command-line editing.

- `fedit filename` — Forks a backup of the file into `.forks/`, then opens the file in your `$EDITOR`.
- `fundo filename` — Restores the last backup from `.forks/` to the working file.

### Why?

Sometimes you just want a lightweight way to back up your file before editing — without the overhead of version control or manual copying.

- Minimal dependencies (Bash, cp, rm, mkdir, ls, sort, awk)
- No git required
- No overhead
- Pure Unix spirit

### Installation

```bash
chmod +x fedit
chmod +x fundo
sudo mv fedit /usr/local/bin/
sudo mv fundo /usr/local/bin/
