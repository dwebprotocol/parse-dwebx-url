# parse-dwebx-url

Node url.parse updated to support versioned dwebx URLs.

```js
var parse = require('parse-dwebx-url')

parse('dwebx://584faa05d394190ab1a3f0240607f9bf2b7e2bd9968830a11cf77db0cea36a21+v1.0.0/path/to/file.txt')
/* => {
  protocol: 'dwebx:',
  slashes: true,
  auth: null,
  host: '584faa05d394190ab1a3f0240607f9bf2b7e2bd9968830a11cf77db0cea36a21',
  port: null,
  hostname: '584faa05d394190ab1a3f0240607f9bf2b7e2bd9968830a11cf77db0cea36a21',
  hash: null,
  search: null,
  query: null,
  pathname: '/path/to/file.txt',
  path: '/path/to/file.txt',
  href: 'dwebx://584faa05d394190ab1a3f0240607f9bf2b7e2bd9968830a11cf77db0cea36a21+v1.0.0/path/to/file.txt',
  version: 'v1.0.0'
}*/
```