# How to consume an API

Interacting with an API is called *consuming* the API. It simply means that you are using the defined methods of the API and sometimes providing some additional data needed by the server to process your request. This additional data is passed in the *params* and the *body* of the *request*, or as an *options* object, depending on the way you call your API.

## Tools

There are several tools you can use to *hit* an API:

- Modern browsers support the [Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch), which allows you to make requests without installing anything else. If you are working with web applications this may be your first option.

- Use an API client, like [Postman](https://www.postman.com/product/api-client/), a very useful tool that allows you to make requests and pass any options using a nice UI.

- Use a command line tool, like [curl](https://curl.se/).

The way you consume an API depends on your needs. For example, if you are developing the front-end of an application that will consume an API, you may use fetch directly from your front-end app. If you don't have a front-end, you can use Postman. Or, if you prefer the command line, you can use curl.

Here are some guides you can follow:

- [Using fetch](https://learning.postman.com/docs/getting-started/sending-the-first-request/)
- [Postman: sending your first request](https://learning.postman.com/docs/getting-started/sending-the-first-request/)
- [Using Curl to make REST API requests](https://linuxize.com/post/curl-rest-api/)
