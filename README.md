# gulp-movilizer-report-pdf
Plugin to ease the generation of the final pdf file from the Movilizer HTML5 Forms framework.

## Config
Add the following task to your `gulpfile.js`:

```javascript
gulp.task('report', ['report.html'], function () {
    return gulp.src('report/*.html')
        .pipe(reportPDF({usePrince:true}));
});
```

## Output
The plugin returns a PDF file with the original name of the HTML input file.

## Options
These options are available in the plugin:

 - jar (optional): specify the location of the [MovilizerHTML2PDF converter tool](https://github.com/Movilizer/movilizer-html2pdf-tool). Default: movilizer-html2pdf-tool.jar
 - usePrince (optional): by default the use of prince as an engine is not enabled

## Requisites
Needed tools:
 - nodejs v5.x.x (https://nodejs.org/)
 - npm v3.x.x (https://www.npmjs.com/)
 - git
 - [MovilizerHTML2PDF converter tool](https://github.com/Movilizer/movilizer-html2pdf-tool) jar
 - (optional) Prince v10.x (https://www.princexml.com)

## Development setup
Open a command line in your projects folder and run the following commands:
```bash
git clone https://github.com/Movilizer/gulp-movilizer-report-pdf.git
cd gulp-movilizer-report-pdf
npm install
```
