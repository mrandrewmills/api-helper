# api-helper
JavaScript object to help fetch responses from API calls as quickly &amp; easily as possible

## Basic Instructions

```JavaScript
// include the api-helper script in your project
<script src="api-helper.js"></script>

// create a new instance of the object
myAPIobj = new apiHelper("https://api.example.com/");

// add any necessary headers
myAPIobj.addHeader("API-Key", "ABC123");

// or Basic Auth Username and Password
myAPIobj.addUsername("");
myAPIobj.addPassword("");

// add URL Parameters
myAPIobj.addParam("state", "Virginia");
myAPIobj.addParam("year", 2020);

// call the API
myAPIobj.fetch();
```  
## Frequently Asked Questions

**1.  How do I remove a header?**

There's a removeHeader() method available. Just pass it the name of the header you want removed.

```JavaScript
myAPIobj.removeHeader("API-Key");
```
**2.  How do I remove a URL Parameter?

There's also a removeParam() method. Just pass it the name of the parameter you wish to remove.

```JavaScript
myAPIobj.removeParam("year");
```
