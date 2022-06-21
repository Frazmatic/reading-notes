# Class 13 Notes

## Why This Matters

Local storage is a useful tool for preserving user information, such as interface settings, and caching information to reduce bandwidth/API call loads. 

## Further Learning

## Questions and Answers:

### [Local Storage and How to Use it on Websites](https://www.smashingmagazine.com/2010/10/local-storage-and-how-to-use-it/)

1. Why would a developer use local storage for a web application?

    Website don't generally store information. Every time you reload/revist a webpage, everything is reset. With local storage, information can be preserved on a user's computer. A program may not have access to a server for storing user information, or may want to reduce use of said servers. Local storage allows a program to store information on a user's computer, and reuse it every time they use the page. Cookies have several limitations that local storage does not. For example, they can only hold 4KB of information, and people disable them for privacy reasons.

2. What information should not be stored in local storage?

    Private information. Information that needs to be secure or encyrypted. 

3. Local storage can store what type of data? How would you convert it to that type before storing it? 

    Local storage can store strings as keys and values. `JSON.stringify()` and `JSON.parse()` methods can be used to convert objects' properties & values to and from strings.

