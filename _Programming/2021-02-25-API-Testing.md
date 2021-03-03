---
title: 'API'
date: 2021-02-23
permalink: /posts/2021/02/restful-api/
tags:
  - API 
---  
- Add Project folder 
- execute `npm install request`
- add `client.js` (https://github.com/request/request#super-simple-to-use)
- modify google website URL into https://reqres.in/api/users 
- `node client.js` 
-  
-  

`client.js` 
```
 1 client.js                                           
 1 const request = require('request');
-  2 request('http://regres.in/api/users', function(error, response, body) {
2  3     console.error('error:', error);
2  4     console.log('statusCode', response && response.statusCode);
2  5     console.log('head:', response.headers);
2  6     console.log('body:', body);
-  7     /** console.log('original format, json format string -----');
3  8      * console.log(body);
3  9      * console.log('translate to JS object---------');
3 10      * console.log(JSON.parse(body));
3 11     **/
2 12 });
```




