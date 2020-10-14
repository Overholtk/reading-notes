## Local Storage

Cookies hold data after a refresh but slow down a page and can't hold enough data to be generally useful

Brief Overview of Previous Methods of Local Storage:
- DHTML behaviors: `userData`
  - can store up to 64KB, or 640KB of data
  
Adobe flash:
- Local shared objects
  - can store up to 100MB briefly, and can be trasmitted to JS with limitations
- ExternalInterface
  - flash 8
  - made it easier to access LSOs
  - gives each domain 100kb of storage

Google:
- Gears in 2007
  - open source browser plugin that provided additional capabilities
  - provides an API to an embedded SQL database
  
All are either specific to a single browser or reliant on a 3rd party plugin...

## HTML5 Storage
- Web Storage, Local Storage, or DOM Storage
  - stores key/value pairs locally within the web browser
  - data persists after you close the page, but is not sent to a remote web server
  - implemented natively in web browsers
 
 Browsers that support HTML5 storage:
 - IE 8.0+
 - Firefox 3.5+
 - Safari 4.0+
 - Chrome 4.0+
 - Opera 10.5+
 - Iphone 2.0+
 - Android 2.0+
 
 Check for HTML5 storage:
  `function supports_html5_storage() {
    try {
      return 'localStorage' in window && window['logalStorage'] !==null;
    } catch (e) {
      return false;
    }
  }`
  
  or
  
    `if(Modernizr.localstorage) {
      //window.localStorage is availible!
     } else {
      // non natice support for HTML5 storage
     }`
     
  Using HTML5 storage:
  - based on key value pairs
  - store and retrieve data based on the key
  - can be any datatype supported by js
  - will always be stored as strings and needs to be altared to the appropriate datatype before use
  - `setItem()` with a key name will enter a value into that key, or overwrite what is already there
  - can be treated as an associative array
  - can be used with both method and bracket notation
  
  Limitations:
  - each origin gets 5MB storage by default
  - "QUOTA_EXCEEDED_ERR" exception is thrown if you exceed the storage quota
  

  
