# How to consume an API

Interacting with an API is called *consuming* the API. It simply means that you are using the defined methods of the API and sometimes providing some additional data needed by the server to process your request. This additional data is passed in the *params* and the *body* of the *request*, or as an *options* object, depending on the way you call your API.

Every API is different, so you should read its documentation before using it. But let's see some examples using a public (no authentication required) API, and the JavaScript *Fetch API*.

**Getting data from an API:**

In your browser **developer tools**, go to the **console** tab and paste this code:

```javascript
fetch('https://jsonplaceholder.typicode.com/todos/1')
  .then(response => response.json())
  .then(json => console.log(json));
```

After some milliseconds, the response will be printed in the console:

```javascript
{ userId: 1, id: 1, title: "delectus aut autem", completed: false }
```

**Sending data to an API:**

Now paste this code:

```javascript
fetch('https://jsonplaceholder.typicode.com/posts', {
  method: 'POST',
  body: JSON.stringify({
    title: 'foo',
    body: 'bar',
    userId: 1,
  }),
  headers: {
    'Content-type': 'application/json; charset=UTF-8',
  },
})
  .then((response) => response.json())
  .then((json) => console.log(json));

```

Now it will print:

```javascript
{ title: "foo", body: "bar", userId: 1, id: 101 }
```

All you need is your browser (or node.js), and the Fetch API!

Note the following:

- Using fetch, the default method is 'GET', you don't need to specify it.
- The return value is a *Promise*, you can use `then()` to handle it when it's resolved.
- When sending data, you must specify the method ('POST', 'PUT', 'PATCH').
- Inside the `body` of the request, you send the data in JSON format.
- Sometimes, you need to specify additional information, like the headers, or in this case specifying the format expected (json).

In these examples, we are using the public [{JSON} Placeholder API](https://jsonplaceholder.typicode.com/), it's free and open, you can use it for testing.

## Tools

There are several tools you can use to *hit* an API. Check them briefly, don't try to understand everything. Right now it is enough to know they exist and that you might use them when needed.

- Modern browsers support the [Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch), which allows you to make requests without installing anything else. If you are working with web applications this may be your first option.

- An API client, like [Postman](https://www.postman.com/product/api-client/) is a very useful tool that allows you to make requests and pass any options using a nice UI. You can also use open source [Hoppscotch](https://hoppscotch.io/) or any other alternative listed in [article "Top 5 Postman alternatives"](https://testfully.io/blog/top-5-postman-alternatives/).

- You can also use a command line tool, like [curl](https://curl.se/).

The way you consume an API depends on your needs. For example, if you are developing the front-end of an application that will consume an API, you may use fetch directly from your front-end app. If you don't have a front-end, you can use Postman. Or, if you prefer the command line, you can use curl.

Here are some guides you can follow:

- [Using fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch).
- [Postman: sending your first request](https://learning.postman.com/docs/getting-started/sending-the-first-request/).

------

_If you spot any bugs or issues in this activity, you can [open an issue with your proposed change](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/git-github/articles/open_issue.md)._
