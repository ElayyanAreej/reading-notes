# Read: 13 - Local Storage

### What we really want is

* a lot of storage space
* on the client
* that persists beyond a page refresh
* and isn’t transmitted to the server

### what is HTML5 Storage?

 Simply put, it’s a way for web pages to **store** named key/value pairs **locally, within the client web browser 🌐**. 
 Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server (unless you go out of your way to send it manually). Unlike all previous attempts at providing persistent local storage, it is implemented natively in web browsers, so it is available even when third-party browser plugins are not.

👉
 **Note**:

 You store data based on a named key, then you can retrieve that data with the same key. The named key is a **string**. 
 So If you are storing and retrieving anything other than strings, you will need to use functions like *parseInt()* or *parseFloat()* to coerce your retrieved data into the expected JavaScript datatype.


 There are also methods for removing the value for a given named key, and clearing the entire storage area.
 ```
 interface Storage {
  deleter void removeItem(in DOMString key);
  void clear();
};
```
 there is a property to get the total number of values in the storage area, and to iterate through all of the keys by index (to get the name of each key).
```
interface Storage {
  readonly attribute unsigned long length;
  getter DOMString key(in unsigned long index);
};
```



“**5 megabytes**” is how much storage space each origin gets by default. 
“QUOTA_EXCEEDED_ERR” is the exception that will get thrown if you exceed your storage quota of 5 megabytes. you Can't ask the user for more storage space At time of writing (February 2011), no browser supports any mechanism for web developers to request more storage space. Some browsers (like Opera) allow the user to control each site’s storage quota, but it is purely a user-initiated action, not something that you as a web developer can build into your web pplication.