# mdBook

## Installation

- Mac

```sh
brew install mdbook
```

- Others: https://github.com/rust-lang/mdBook/releases

### Test installation

```sh
mdbook
```

Creating a book

```sh
mdbook init my-book
```

```sh
Do you want a .gitignore to be created? (y/n)
y
What title would you like to give the book?
My Book
2022-02-01 09:35:54 [INFO] (mdbook::book::init): Creating a new book with stub content
```

## Rendering a book

```sh
cd my-book
```

### Serve a book

```sh
mdbook serve
```

```sh
## start and open web browser
mdbook serve --open
```

## mdBook Settings

### A book settings

book.toml

```sh
[book]
authors = ["your name"]
language = "en"
multilingual = false
src = "src"
title = "My Book"
```

### A book layout

SUMMARY.md: A list of all chapters in the book.
src/SUMMARY.md

```sh
# Summary

- [Chapter 1](./chapter_1.md)
```

## Create and Edit Content

### Create new chapter

Append the following line to SUMMARY.md

```
- [Chapter 2](./chapter_2.md)
```

```
# Summary

- [Chapter 1](./chapter_1.md)
- [Chapter 2](./chapter_2.md)
```

> Refresh the web browser

### Edit content

Open chapter_1.md with your text editor

1. Header

   Append the following line to chapter_1.md

   ```sh
   ## Header
   ```

2. New line

   Append the following line to chapter_1.md

   ```sh
   first line
   second line
   ```

   > first line[enter two spaces]

3. Unordered list

   Append the following line to chapter_1.md

   ```sh
   - first bullet
   - second bullet
   ```

4. Ordered list

   Append the following line to chapter_1.md

   ```sh
   1. first item
   2. second item
   ```

5. Code

   Append the following line to chapter_1.md

   ```sh
   `code`
   ```

6. Bold text

   Append the following line to chapter_1.md

   ```sh
   **bold text**
   ```

7. Image

   Append the following line to chapter_1.md

   ```sh
   ![markdown](https://alternativetoapp.com/wp-content/uploads/2020/05/mdbook_158088.png)
   ```

8. Link

   Append the following line to chapter_1.md

   ```sh
   [Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet/)
   ```

e.g. chapter_1.md

```md
# Chapter 1

## Header

first line  
second line

- first bullet
- second bullet

1. first item
2. second item

`code`

**bold text**

![markdown](https://alternativetoapp.com/wp-content/uploads/2020/05/mdbook_158088.png)

[Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet/)
```
