### Gulp

##### gulpfile.js


    var gulp = require('gulp'),
        flatten = require('gulp-flatten'),
        dirs = {
            bower: 'src/main/webapp/static/bower_components',
            dest: 'src/main/webapp/dist',
        };

    gulp.task('copy:fonts', function () {
        gulp.src(dirs.bower + '/**/*.{ttf,woff,eof}')
            .pipe(flatten())
            .pipe(gulp.dest(dirs.dest + '/fonts'));
    });

    gulp.task('default', function () {
        runSequence('copy:fonts');
    });
    
