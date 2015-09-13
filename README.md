# simple-sticky-header

Very simple javascript &amp; CSS fixed header on scroll down based on an element's height.

Pure vanilla javascript with no dependencies. Add a "fixed" class on an identified div element (#header) which allow to fix it when visitors scroll down on a web page. Calculations are made automaticaly based on the height of this #header. Simply copy/past: you just need to add a CSS declaration into your styles file (i.e.: .fixed{position:fixed}).

## HTML markup

    <div class="header-outer" id="menu">
      <div class="header-inner" id="header">
        Header
      </div>
    </div>

Note: IDs "menu" & "header" are needed.

## Options

> `down`: distance in pixels from the top of the page where to apply the fixed element. Default: the #header's height.
> 
> `up`: distance in pixels from the top of the page where to stop the fixed element. Default: the #header's height.
>
> `delay`: timeout in milliseconds. Default: 70.

## Script loader

Call this script with its `function fixednav()` and set options as needed:

    fixednav({down:50, up:200, delay:70});

Check out: [this online demo (new version)](http://jsfiddle.net/gtcL1cmm/7/).

Check out: [this online demo (old version)](http://jsfiddle.net/gtcL1cmm/2).
