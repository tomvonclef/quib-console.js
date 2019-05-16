quib-console.js
================

This is a javascript HTML5 canvas console based on code taken from
the excellent qb.js (http://stevehanov.ca/blog/index.php?id=92).

It translates the original QBasic console commands into an API.

This version has HiDPI support. By using 2x-scaled images, it avoids
HTML5 canvas fuzziness that otherwise occurs when scalingup the glyph images.

It supports all characters from code page 437.
See also: https://en.wikipedia.org/wiki/Code_page_437. 
In particular, qb.js does not include smile characters, but I
have added those!

## Example

```js
   const cons = new Console(2);    // 2 for 2x scaling (for HiDPI displays)
   cons.print("Hello World");
```

## Functions
+ backup: function( num )
+ circle: function( x, y, radius, colour, start, end, aspect, step )
+ cls: function()
+ color: function( fg, bg )
+ cursor: function( show )
+ enableCursor: function( enabled )
+ get: function( x1, y1, x2, y2, step1, step2 )
+ getKeyFromBuffer: function()
+ input: function( onInputDone )
+ line: function( x1, y1, x2, y2 )
+ lineTo: function( x, y )
+ locate: function( row, col )
+ newline: function()
+ onKeyDown: function( event )
+ paint: function( x, y, colour, borderColour, step )
+ print: function( str )
+ printError: function(str)
+ put: function( data, x, y )
+ record: function(str)
+ reset: function(testMode)
+ screen: function( num )
+ scroll: function()
+ setKeyBuffer: function( str )
+ toggleCursor: function()

