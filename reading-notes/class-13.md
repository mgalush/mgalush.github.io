# Local Storage

Cookies can be used to store small amounts of data, but have three downsides: 
1. They are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
2. They are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
3. They are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful

### HTML5 storage, aka **local storage** or **DOM storage** is a way for a webpage to store named key/value pairs

Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server

You can access it through the `localStorage` object on the global `window` object

*Note: all data is stored as a string*

To receive anything other than a string, use the functions `parseInt()` or `parseFloat()`

### HTML5 local storage limitations:
You can only store 5 megabytes and will receive the “QUOTA_EXCEEDED_ERR” exception if you exceed it.  Because integers or floats are stored as the character representations and not the actual number, you can reach this 5 Mbt limit fairly quickly