### Why?

Why does running the same command through `npm` result in different files being parsed?

```bash
$ node node_modules/.bin/js-beautify -rn *.js lib/**/*.js
beautified index.js - unchanged
beautified lib/index2.js - unchanged
beautified lib/sub/index3.js - unchanged

$ npm run beautify

> npmglob@1.0.0 beautify /Users/drew/Projects/self/npmglob
> js-beautify -rn *.js lib/**/*.js

beautified index.js - unchanged
beautified lib/sub/index3.js - unchanged
```
