# Bookshelf

Bookshelf is a Python utility to generate static HTML bookshelves.

## Install

Packaging is still TODO

## Input data

The input data is a csv file with your books in the following format:

```
title,author,isbn,asin,rating,date_finished
Animal Farm,George Orwell,0452284244,,4,2018-01-23 05:12:03
```

ISBN and ASIN are used to retrieve the book's cover from the [Open Library
Cover API](https://openlibrary.org/dev/docs/api/covers).

## Running

```
./bookshelf <config file>
```

## Config file

For example:

```json
{
    "build": "build",
    "theme": "themes/default",
    "books": "books.csv",
    "title": "Bookshelf"
}
```

## License

GPLv3
