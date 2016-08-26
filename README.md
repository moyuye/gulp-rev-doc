# gulp-rev-doc
gulp插件，静态资源加版本号。

# View
before
```html
<link href="abc.css" rel="stylesheet">
<script type="text/javascript" src="abc.js"></script>
<img src="abc.jpg" width="176" height="106" alt="" />
```

after
```html
<link href="abc.css?v=c689073d22c3" rel="stylesheet">
<script type="text/javascript" src="abc.js?v=be3c502107d9"></script>
<img src="abc.jpg?v=a96086485c4d" width="176" height="106" alt="" />
```

# Usage
```bash
npm install gulp-rev-doc --save-dev
```

```js
var revDoc = require('gulp-rev-doc');

gulp.task('default', function() {
    return gulp.src('./src/**/*.html')
        .pipe(revDoc())
        .pipe(gulp.dest('./src'))
});
```

# Links
- NPM: https://www.npmjs.com/package/gulp-rev-doc
- Bug：https://github.com/kyo4311/gulp-rev-doc/issues
- Myblog：http://www.f00sun.com

# License

MIT