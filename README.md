# Linux for Creators: Pop!_OS from Beginner to Advanced
This project *intends* to be a user manual for [Pop!_OS](https://pop.system76.com/) by [System76](https://system76.com/), but I am just getting started.

### A note about licensing
I have not worked out the details on how this book will be licensed for mass distribution. I fully intend for it to be some form of *copyleft*, but I do not know under what terms. During production it will be free (as in beer), but all other rights are reserved.

### Create Book
1. Install [Pandoc](https://pandoc.org/).
2. Clone this repository to your local machine.
3. Build the book with the following syntax:
```bash
pandoc -s --toc --epub-embed-font='fonts/*.ttf' -o book.epub metadata.txt \
    ./00-Front-Matter/00-Front-Matter.md \
    ./00-Introduction/00-Introduction.md \
    ./99-Back-Matter/99-Back-Matter.md
```

Your book will be exported as `book.epub`.
