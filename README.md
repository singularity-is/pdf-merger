# PDF Merger

[![Latest Version](https://img.shields.io/github/tag/singularity-is/yii2-daterangepicker.svg?style=flat-square&label=release)](https://github.com/singularity-is/pdf-merger/tags)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE.md)
[![Build Status](https://img.shields.io/travis/singularity/yii2-daterangepicker/master.svg?style=flat-square)](https://travis-ci.org/singularity/pdf-merger)
[![Coverage Status](https://img.shields.io/scrutinizer/coverage/g/singularity/yii2-daterangepicker.svg?style=flat-square)](https://scrutinizer-ci.com/g/singularity/pdf-merger/code-structure)
[![Quality Score](https://img.shields.io/scrutinizer/g/singularity/yii2-daterangepicker.svg?style=flat-square)](https://scrutinizer-ci.com/g/singularity/pdf-merger)
[![Total Downloads](https://img.shields.io/packagist/dt/singularity/yii2-daterangepicker.svg?style=flat-square)](https://packagist.org/packages/singularity/pdf-merger)


## Installation

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```bash
$ composer require singularity/pdf-merger:~1.0
```

or add

```
"singularity/pdf-merger": "~1.0"
```

to the `require` section of your `composer.json` file.

## Usage
```
include 'PDFMerger.php';

$pdf = new PDFMerger;

$pdf->addPDF('samplepdfs/one.pdf', '1, 3, 4') specific pages
	->addPDF('samplepdfs/two.pdf', '1-2') range of pages
	->addPDF('samplepdfs/three.pdf', 'all') all pages
	->merge('file', 'samplepdfs/TEST2.pdf');

```
	//REPLACE 'file' WITH 'browser', 'download', 'string', or 'file' for output options
	//You do not need to give a file path for browser, string, or download - just the name.


## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Credits

- [Nikola Radovic](https://github.com/dzona)
- [All Contributors](https://github.com/singularity-is/pdf-merger/graphs/contributors)

## License

The BSD License (BSD). Please see [License File](LICENSE.md) for more information.


<a href="https://singularity.is"><img src="http://www.gravatar.com/avatar/8663d48ea6093d2ce917217ceeca1cc2.png"></a><br>
<i>#InventTomorrow</i><br>
<a href="https://www.singularity.is">www.singularity.is</a>
