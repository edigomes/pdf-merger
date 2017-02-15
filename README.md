#PDFMerger for PHP (PHP 5 or 7 Compatible)

Original written by http://pdfmerger.codeplex.com/team/view<br />
Forked from https://github.com/myokyawhtun/PDFMerger

## Composer Compatible

I've just forked this package to make it compatible with composer and work with pdf from URL
To install add this line to your composer.json

```"edigomes/pdf-merger": "dev-master"```

### Example Usage
```php

$pdf = new \Clegginabox\PDFMerger\PDFMerger;

$pdf->addPDF(file_get_contents('http://beta.local/test1.pdf'));
$pdf->addPDF(file_get_contents('http://beta.local/test2.pdf');

$pdf->merge('file', 'samplepdfs/TEST2.pdf', 'P');

// REPLACE 'file' WITH 'browser', 'download', 'string', or 'file' for output options
// Last parameter is for orientation (P for protrait, L for Landscape). 
// This will be used for every PDF that doesn't have an orientation specified
```
