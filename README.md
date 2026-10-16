<div align="center">

# 🚀 jj

**Find a file. Jump straight to it.**

A generic, friendlier take on `find | grep` — fuzzy-search your files and `cd` right into them.

![Shell](https://img.shields.io/badge/shell-bash-4EAA25?logo=gnubash&logoColor=white)
![Platform](https://img.shields.io/badge/platform-Linux-blue?logo=linux&logoColor=white)
![Requires](https://img.shields.io/badge/requires-fzf-orange)

<!-- Replace with your own demo GIF: docs/images/demo.gif -->
<img src="docs/images/demo.gif" alt="jj demo" width="720">

</div>

## ✨ Features

- ⚡ **Fast** – lists files under the current directory and filters as you type
- 🔍 **Fuzzy search** – powered by [fzf](https://github.com/junegunn/fzf), no regex needed
- 🧭 **Instant jump** – `cd` into the selected directory, or the directory containing the selected file
- 🪶 **Tiny** – a single shell function, no dependencies besides `fzf`

## 📦 Installation

1. Install [fzf](https://github.com/junegunn/fzf) (e.g. `sudo apt install fzf`).
2. Append the contents of [`jj/jj.txt`](jj/jj.txt) to the bottom of your `~/.bashrc`:

   ```bash
   cat jj/jj.txt >> ~/.bashrc
   source ~/.bashrc
   ```

## 🎯 Usage

```bash
jj            # browse everything below the current directory
jj notes      # start with "notes" pre-filled in the query
```

Pick an entry with <kbd>Enter</kbd> (cancel with <kbd>Esc</kbd>) and your shell jumps there:

```text
$ jj readme
selected: ./docs/README.md
/home/user/project/docs
```

## 🖼️ Screenshots

| Search | Jump |
|:------:|:----:|
| ![search](docs/images/search.png) | ![jump](docs/images/jump.png) |

### Adding your own images

1. Put image files (PNG, JPG, GIF) in [`docs/images/`](docs/images/).
2. Reference them with a relative path in Markdown:

   ```markdown
   ![alt text](docs/images/screenshot.png)
   ```

3. To control size, use HTML:

   ```html
   <img src="docs/images/demo.gif" alt="demo" width="600">
   ```

4. Commit and push — GitHub renders them automatically. Tip: record GIFs with tools like [asciinema](https://asciinema.org/) + [agg](https://github.com/asciinema/agg), or [peek](https://github.com/phw/peek).

> Until real images are added, the image links above will appear broken.

## 💻 System Requirements

- Linux (developed on Linux Mint 22.3 MATE)
- bash and `fzf`

## 📄 License

See [LISENCE](LISENCE).
