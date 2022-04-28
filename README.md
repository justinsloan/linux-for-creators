# Linux for Creators: Pop!_OS from Beginner to Advanced
This project *intends* to be a user manual for [Pop!_OS](https://pop.system76.com/) by [System76](https://system76.com/), but I am just getting started.

### Licensing and Distribution
This book is licensed under the Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0) [license](https://creativecommons.org/licenses/by-sa/4.0/).

*Linux for Creators* is not affiliated with or endorsed by Canonical, Ltd. or System76, Inc.

### How to Build/Create the Book
1. Install [Pandoc](https://pandoc.org/).
2. Clone this repository to your local machine.
3. Build the book with the following syntax:
```bash
pandoc -s \
    --toc --toc-depth=2 \
    -V toc-title:"Table of Contents" \
    --epub-embed-font='fonts/*.ttf' \
    -f markdown+implicit_figures \
    -o book.epub \
    metadata.txt \
    ./00-Front-Matter/00-Front-Matter.md \
    ./00-Introduction/00-Introduction.md \
    ./01-Installing-Pop-OS/01-Installing-Pop-OS.md \
    ./02-The-COSMIC-Desktop/02-The-COSMIC-Desktop.md \
    ./03-Using-the-Terminal/03-Using-the-Terminal.md \
    ./04-Finding-and-Installing-Applications/04-Finding-and-Installing-Applications.md \
    ./05-System-Administration/05-System-Administration.md \
    ./06-Customizing-Pop-OS/06-Customizing-Pop-OS.md \
    ./07-Advanced-Customization/07-Advanced-Customization.md \
    ./08-Gaming-on-Linux/08-Gaming-on-Linux.md \
    ./09-The-Pop-OS-Community/09-The-Pop-OS-Community.md \
    ./99-Back-Matter/99-Back-Matter.md
```

Your book will be exported as `book.epub`.
