This is a vanilla JavaScript application that fetches random facts on any number entered. 

I used both XHR and the Fetch API to make requests to http://numbersapi.com
As well as a bit of bootstrap for styling.

In the code I've commented out the the XHR request as i wanted to demonstrate that you can use XHR or Fetch to achieve the same thing.

In my opinion it's better to use Fetch because there are a few things that you can do with fetch and not with XHR:

You can use the Cache API with the request and response objects.

You can perform no-cors requests(Cross origin resource sharing), getting a response from a server that doesn't implement CORS. You can't access the response body directly from JavaScript, but you can use it with other APIs (e.g. the Cache API);

Streaming responses with XHR the entire response is buffered in memory, with fetch you will be able to access the low-level stream. 

However there are a few things that you can do with XHR that you can't do yet with Fetch such as report progress.
