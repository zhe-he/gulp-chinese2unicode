# 基于gulp的将文件中的中文转换成unicode编码的插件

## 用法

```javascript
chinese2unicode([encoding])
```

## 例子

```javascript
var gulp = require('gulp');
var chinese2unicode = require('gulp-chinese2unicode');
gulp.task('chinese2unicode', function() {
    return gulp.src('./source/test.js')
                .pipe(chinese2unicode())
                .pipe(gulp.dest('./dest/'));
});
```


## 参数

### encoding string(可选)

如果你明确知道文件的编码，可以添加encoding参数，如果不设置，插件会自动检测编码。	

##其他	
[github](https://github.com/zhe-he/gulp-chinese2unicode)	
[建议](https://github.com/zhe-he/gulp-chinese2unicode/issues)