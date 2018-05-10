# simple-sticky-header

Very simple javascript &amp; CSS fixed header on scroll down based on an element's height.

Pure vanilla javascript with no dependencies. Add a "fixed" class on an identified div element (#header) which allow to fix it when visitors scroll down on a web page. Calculations are made automaticaly based on the height of this #header. Simply copy/past: you just need to add a CSS declaration into your styles file (i.e.: .fixed{position:fixed}).

## HTML markup

    <div class="header-outer" id="header-outer">
      <div class="header-inner" id="header">
        Header
      </div>
    </div>

Note: IDs `header-outer` & `header` are needed (can be changed for other identifiants, see **options** below).

## Options

> `down`: distance in pixels from the top of the page where to apply the fixed element. Default: the #header's height.
> 
> `up`: distance in pixels from the top of the page where to stop the fixed element. Default: the #header's height.
>
> `delay`: timeout in milliseconds. Default: 70.

## Script loader

Call this script with its `function fixednav()` and set options as needed:

    fixednav({id:"inner-id", outer:"outer-id", distance:40, down:50, up:200, delay:70});

## Attributes

>    `id`: ID of the inner element of the header.
> 
>    `outer`: ID of the outer element of the header.
> 
>    `distance`: (optional) distance in pixel from the top of the browser's window where to apply the fixed position. Default: the menu element height.
> 
>    `down`: (optional) additional down distance in pixel when to apply the fixed position. Default: 0.
> 
>    `up`: (optional) additional up distance in pixel when to remove the fixed position. Default: 0.
> 
>    `delay`: (optional) delay in ms. Default: 70 ms.

Check out: [this online demo (new version)](http://jsfiddle.net/gtcL1cmm/9/).

Check out: [this online demo (old version)](http://jsfiddle.net/gtcL1cmm/2).
