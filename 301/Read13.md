# Sending Form Data

## Client/server architecture
- client sends a request to server using HTTP, then the server answers the same way
- HTML configures HTTP

## Defining how to send the data
- form element defines how the data will be sent
- action: defines where the data gets sent
  - if a url is not provided, data will be sent to the current page
- method: defines how data is sent
  - GET: method used by the browser to ask the server to send back a given resource
  - ? followed by name/value pairs, then & to separate each pair
  - POST: talks to the server when asking for a response that takes HTTP data into account
  - data is not appended to the URL, included in request body instead
- HTTP request can be viewed in developer tools

## Retrieving the Data:
- PHP offers global objects to access data

## Sending Files:
- enctype lets you specify the Content-Type
- Three extra steps to send files:
  - method to POST
  - enctype to multipart/form-data
  - <input type="file">
