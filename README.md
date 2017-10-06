# PDF Merge for PHP

PDF Merge library for PHP.

A fork of "jurosh/pdf-merge"
This was done to use setasign licensed code.

Install in composer:

```json
"reprovinci/pdf-merge": "dev-master"
```

## Highlights

Pdf merging with modes portrait/landscape.

Tested in Laravel4 & Laravel5 framework (but still can be used without any framework as standalone utility).

## Usage

```php
// Autoload classses...

// and we can do stuff
$pdf = new \Jurosh\PDFMerge\PDFMerger;

// add as many pdfs as you want
$pdf->addPDF('path/to/source/file.pdf', 'all', 'vertical')
  ->addPDF('path/to/source/file1.pdf', 'all')
  ->addPDF('path/to/source/file2.pdf', 'all', 'horizontal');

// call merge, output format `file`
$pdf->merge('file', 'path/to/export/dir/file.pdf');
```
