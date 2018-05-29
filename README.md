# mini-code
Barcode and QRCode for miniprogram plugin.

![](https://img.shields.io/badge/Build-Passing-brightgreen.svg) ![](https://img.shields.io/badge/License-MIT-lightgrey.svg) 

## Install
Install with [npm](https://www.npmjs.com/):

```sh
$ npm install --save mini-code
```
## Usages
``` js
var QRCode = require('mini-code').QRCode

QRCode.draw({
    canvas: '', //canvas context
    code: '', //code
    width: 300, //qrcode width
    height: 300,
    iconImg: '', // icon url. @optional
    iconWidth: 60, //icon width. @optional
    iconHeight: 60, 
},
{//@optional. draw qrcode with scale animation.
    duration: 300,
    scale: 0.8
})

var BarCode = require('mini-code').BarCode

BarCode.draw({
    canvas: '',//canvas context
    code: '',//code
    width: '',//barcode width
    height: '',//barcode height
    vertical: false //show barcode in vertical case.
})
```