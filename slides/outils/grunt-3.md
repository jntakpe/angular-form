### Grunt

##### gruntfile.js

    {
    module.exports = function (grunt) {
        grunt.initConfig({
            pkg: grunt.file.readJSON('package.json'),
            concat: {
                libs: {
                    src: [
                        'js/jquery/dist/jquery.min.js',
                        'js/angular/angular.min.js'
                    ],
                    dest: 'target/js-libs.min.js'
                }
            }
        });
        grunt.loadNpmTasks('grunt-contrib-concat');
        grunt.registerTask('default', ['concat:libs']);
    }
