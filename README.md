https://user-images.githubusercontent.com/81305164/152664895-8c1ad584-eea9-4cb2-8baa-4c27c09eb8a3.mp4

# manga-cli

Bash script for reading mangas via the terminal by scraping [manganato](https://manganato.com/)

## Table of Contents

- [Usage](#Usage)
- [Install](#Install)
- [Dependencies](#Dependencies)
- [Preview](https://user-images.githubusercontent.com/81305164/152664895-8c1ad584-eea9-4cb2-8baa-4c27c09eb8a3.mp4)
- [Disclaimer](./DISCLAIMER.md)
- [License](./LICENSE.md)

## Usage

```text
Bash script for reading mangas via the terminal

Usage:
	manga-cli [Option] [Manga Name]

Options:
	-h, --help		Print this help page
	-V, --version		Print version number
	-u, --update		Fetch latest version from the Github repository
	-f, --fullscreen	Open Zathura in fullscreen mode 
	-vv, --vertical 	Create all pdf images of the same size vertically
	-hh, --horisontal	Create all pdf images of the same size horisontally
	-l, --last-session    	Open last session
	-c, --cache-size	Print cache size ($HOME/.cache/manga-cli)
	-C, --clear-cache	Clear cache ($HOME/.cache/manga-cli)
```

## Install

### Arch Linux

Use the AUR helper of your choice or install [manga-cli-git](https://aur.archlinux.org/packages/manga-cli-git) manually

Use the following commands when using yay or paru:

```sh
yay -S manga-cli-git
```

```sh
paru -S manga-cli-git
```

### Linux

Install dependencies [(See below)](#Dependencies)

```sh
git clone https://github.com/7USTIN/manga-cli && cd manga-cli
sudo cp manga-cli /usr/local/bin/manga-cli
```

## Dependencies

- GNU coreutils (ls, tr, rm, du, cat, mkdir)
- GNU diffutils (diff)
- GNU patch
- GNU gawk (awk)
- GNU sed
- curl
- git
- img2pdf
- zathura
- zathura-pdf-mupdf **OR** zathura-pdf-poppler
