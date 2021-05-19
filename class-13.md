# Lecture Notes 13

## All about Local Storage
- Diving in
- Brief History
- HTML5 Storage
- Beyond named key-value pairs: competing visions

### Diving in
- native client apps have held advantages over web apps for local storage.
- If you need local storage beyond just key-value pairs in native, just embed a database.
- Cookies:
  - Web apps use them to hold local storage
  - Cookies are included with every HTTP request, slowing down the web by transmitting same data
  - sends unencrypted data over the internet.
  - Limited to 4kb of data. Not very much.

- What to look for in local storage
  - lots of storage space
  - on the client
  - persists beyond page refresh
  - isn't transmitted to server.

### A history: 
- userData, hierarchical XML-based structure
- Adobe Flash 5 "Flash cookies". Can store up to 100kb of data per domain.
- Google "gears" 2007, open source browser plugin. Gears provides API to embedded SQL database based on SQLite
- HTML5 wanted to give a standard API that all browsers could use.

### HTML5 Storage
- A specification named Web storage, at one time part of HTML5 specification proper but split out into own specification.
- What is it? 
  - A way for web pages to store named key/value pairs with client web browser.
  - Like cookies, data persists.
  - The data is never transferred to the server.
  - Implemented natively in browsers.
- Using HTML5 storage.
  - Store data based on a named key, then retrieve that data with same key.
  - Storage events  can be tracked with storage changes, such as removeItem(), clear().
  
#### Beyond named key-value pairs:
- A new API has been standardized and implemented across all major browsers, platforms and devies.
- Google gears is one of the "futures" of local storage.
  - an embedded database based on SQLite that is localstorage.
  - later influced creation of Web SQL Database. Provides thin wrapper around SQL database.
  ``` js
openDatabase('documents', '1.0', 'Local document storage', 5*1024*1024, function (db) {
  db.changeVersion('', '1.0', function (t) {
    t.executeSql('CREATE TABLE docids (id, name)');
  }, error);
});
  ```
- Another competing vision for local storage is Indexed Database API, "IndexedDB" or "WebSimpleDB"

