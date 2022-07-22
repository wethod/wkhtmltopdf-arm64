wkhtmltopdf-arm64
================

This repository contains the static compiled binaries from the [wkhtmltopdf project](http://wkhtmltopdf.org/) on arm64 architecture.
More about the functionality of wkhtmltopdf and wkthmltoimage can be found there.

## Installation

``` json
{
    "require" {
        "wethod/wkhtmltopdf-arm64": "master",
    },
    "repositories": [
        {
            "type": "git",
            "url": "https://github.com/wethod/wkhtmltopdf-arm64"
        },
    ],
}
```

### Usage

You can use the path constant to easily locate the binary in the PHP codebase: 

``` php
$path = \wethod\WKHTMLToPDF\WKHTMLToPDF::PATH;
```

For realpath use following script

``` php
$realpath = realpath(\wethod\WKHTMLToPDF\WKHTMLToPDF::PATH);
```
