# Awesome books: plain JS with objects

## Learning objectives
- Use JavaScript objects as design pattern.
- Use developer tools to print information to the console.

### Estimated time: 3h

## Description
You will learn how to use JS objects to add/remove books and update the books list accordingly.

### Project requirements
- Add new book with title and author (newly added book should be displayed on the list)
- Remove a book from the list (it should disappear from the list).

Remember the basic design of our books application:
![Awesome books basic UI](./images/awesome_books_basic_ui.png "Awesome books basic UI")

To add a book, you can represent it as an **object**, to do that you need to identify the data you need, in this case, the `title`, `author` and since several books can have the same author or title you need a unique `id` to identify each book. Your object should look like this:

```javascript
const book = {
  title: "Lorem ipsum",
  author: "Testeroo Testyy",
  id: 1
}
````

Then, you need a place to store all your books, you can do this with an **array**:

```javascript
const books = [] // At the beginning is empty
books.push(book) // push will add your book to the array of books
```

To see in the console the last change you've made to the array, use **console.log()**:

```javascript
console.log(books)
```

To access the books stored in your books array, you can access them with its index:

```javascript
const firstBook = books[0] // Arrays are zero-based, 0 is the first element
console.log(firstBook.title) // Access the property title in your object
```

Or, you can iterate over the entire collection:

```javascript
for(let book of books){
  console.log(book)
}
```

To **remove** a single book from the book list, you need to filter using the unique identifier `id`. There are several ways to do this, one is using the array **filter()** method:

```javascript
const filteredBooks = books.filter(book => book.id !== 1) // Will return a new array whit all the books where id is not 1
```

To save your books in the browser's memory, you can use **localStorage**, remember that localStorage supports only string values, not arrays or objects, you'll need to use **JSON.stringify()** and **JSON.parse()**:

```javascript
localStorage.setItem("books", JSON.stringify(books)) // Saving to local storage
const storedBooks = JSON.parse(localStorage.getItem("books")) // Get an item from local storage
```

Take a look at this useful **documentation**:

[MDN - Working with objects](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects)

[MDN - Aray](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)

[MDN - Array.prototype.filter()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter)

[MDN - console.log()](https://developer.mozilla.org/en-US/docs/Web/API/Console/log)

[MDN - Window.localStorage](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage)

[MDN - JSON](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/JSON)
