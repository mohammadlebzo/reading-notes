# Local Storage

## Brief History of Local Storage Hacks Before HTML5
At first there was only **Internet Explorer**, a browser that was invented by **Microsoft**, with many great things to end the all browser wars at that time.

One of these things was called **DHTML Behaviors**, and one of these behaviors was called **userData**, which allows webpages to store up to 64 KB of data per domain.

Then in 2002, **Adobe** introduced **"Flash cookies"** as a feature in **Flash 6**, known as **Local Shared Object**, which allows flash objects to store up to 100 KB of data per domain.

After that in 2007, **Google** launched **Gears**, an open source browser plugin aimed to provide additional capabilities in browsers Gears provides an API to an embedded SQL database based on SQLite After obtaining permission from the user once, Gears can store unlimited amounts of data per domain in SQL database tables.

The problem is that there was a pattern in these solutions, it was that all of them are either specific to a single browser, or relaint on a **third-party plugin**, and because of that, **Brad Neuberg** and others continued to hack away on **dojox.storage** to provide a unified interface to all these different plugins and APIs.

By 2009, dojox.storage could auto-detect (and provide a unified interface on top of) Adobe Flash, Gears, Adobe AIR, and an early prototype of HTML5 storage that was only implemented in older versions of Firefox.

And after understanding this problem HTML5 was set out to solve it, to provide a standardized API, implemented natively and consistently in multiple browsers, without having to rely on third-party plugins.

## What is HTML5 Storage ?
**HTML5 Storage** is a way for web pages to store named key/value pairs *locally*, within the **client web browser**. Like **cookies**, this data persists even after you *navigate away from the web site*, *close your browser tab*, *exit your browser*, or what have you. **Unlike cookies**, this data is **never** transmitted to the *remote web server* (unless you go out of your way to send it manually). Unlike all previous attempts at providing persistent local storage, it is implemented **natively in web browsers**, so it is available even when **third-party** browser **plugins** are not.

**Note**: you can use **Modernizr** to detect support for HTML5 Storage.

## Using HTML5 Storage

When using the **HTML5 Storage** all data types that are supported by **JavaScript** can be used, however data will be stored only as ***strings***. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloa() to coerce your retrieved data into the expected JavaScript datatype.

***Some Methods***:

- Calling **setItem()** with a named key that already exists will silently overwrite the previous value.

- Calling **getItem()** with a non-existent key will return null rather than throw an exception.

- Calling **removeItem()** with a non-existent key will do nothing.

- Calling **key()** gets the total number of values in the storage area, and you can iterate through all of the keys by using the index of the key.

**Note**: If you call ***key()*** with an index that is not **between 0–(length-1)**, the function will return null.

## Tracking Changes To The HTML5 Storage Area

If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something. For example, if you set an item to its existing value or call clear() when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area.

## Limitations 

- **5 megabytes per origin by default**.
- **Getting "QUOTA_EXCEEDED_ERR" as an exception whenever you exceed the storage quata of 5 magabytes**.
- Your unable to ask the user for more storage space