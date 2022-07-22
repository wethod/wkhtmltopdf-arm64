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

## Usage

You can use the path constant to easily locate the binary in the PHP codebase: 

``` php
$path = \wethod\WKHTMLToPDF\WKHTMLToPDF::PATH;
```

For realpath use following script

``` php
$realpath = realpath(\wethod\WKHTMLToPDF\WKHTMLToPDF::PATH);
```

## How to retrive binaries

Download binary from [https://wkhtmltopdf.org/downloads.html](https://wkhtmltopdf.org/downloads.html), then unpack the .deb file and get the executable with:

``` bash
ar x wkhtmltopdf-arm64.deb
unxz data.tar.xz
mkdir data/
tar -xvf data.tar -C data/
ls data/usr/local/bin/wkhtmltopdf
```

Binary are now in `data/usr/local/bin/wkhtmltopdf`
