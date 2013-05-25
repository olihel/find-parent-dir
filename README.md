# find-parent-dir [![build status](https://secure.travis-ci.org/thlorenz/find-parent-dir.png)](http://travis-ci.org/thlorenz/find-parent-dir)

Finds the first parent directory that contains a given file or directory.


    npm install find-parent-dir

```js
// assuming this is called from a file in a subdirectory of /myprojects/foo which contains .git directory
var findParentDir = require('find-parent-dir');

findParentDir(__dirname, '.git', function (err, dir) {
  // has err if some file access error occurred
  console.log(dir); // => /myprojects/foo/
})
```
