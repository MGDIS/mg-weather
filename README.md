mg-weather
==========

This font gathers a set of icons about weather. It has been initialy created by **FONTELLO** using some icons from different fonts. Content of the fonts can be seen on the demo page.

Demo
-----------------------
![alt tag](https://cloud.githubusercontent.com/assets/8104134/5067910/6b5b8454-6e48-11e4-952d-0a53dfe78d34.png)

Useful files
-----------------------

- /font/* - fonts in different formats

- /css/*  - different kinds of CSS, for all situations. Should be ok with 
  twitter bootstrap. Also, you can skip <i> style and assign icon classes
  directly to text elements, if you don't mind about IE7.

- demo.html - demo file, to show the webfont content

Why so many CSS files ?
-----------------------

Because we pride ourselves with fitting all your needs :)

- basic file, <your_font_name>.css - is usually enough, it contains @font-face
  and character codes definition

- *-ie7.css - if you need IE7 support, but still don't wish to put char codes
  directly into html

- *-codes.css and *-ie7-codes.css - if you like to use your own @font-face
  rules, but still wish to benefit from css generation. That can be very
  convenient for automated assets build systems. When you need to update font -
  no need to manually edit files, just override old version with archive
  content. See fontello source codes for example.

- *-embedded.css - basic css file, but with embedded WOFF font, in order to avoid
  CORS issues in Firefox and IE9+, when fonts are hosted on the separate domain.
  We strongly recommend to resolve this issue by `Access-Control-Allow-Origin`
  server headers. But if you are fine with a dirty hack - this file is for you.
  Please note that data url is moved to separate @font-face to avoid problems with <IE9,
  when the string is too long.

- animate.css - use it to get ideas about spinner rotation animation.


Attention for server setup
--------------------------

You MUST setup server to reply with proper `mime-types` for font files. If not,
some browsers will fail in showing fonts.

Usually, `apache` already has necessary settings, but `nginx` and other
webservers should be tuned. Here is list of mime types for our file extentions:

- `application/vnd.ms-fontobject` - eot
- `application/x-font-woff` - woff
- `application/x-font-ttf` - ttf
- `image/svg+xml` - svg

Credits
--------------------
mg-weather is created from a selection of those fonts  

  * Typicons

   Author:    **Stephen Hutchings**  
   License:   SIL (http://scripts.sil.org/OFL)  
   Homepage:  http://typicons.com/  


  * Meteocons

   Author:    **Alessio Atzeni**  
   License:   SIL (http://scripts.sil.org/OFL)  
   Homepage:  http://www.alessioatzeni.com  


  * Iconic

   Author:    **P.J. Onori**  
   License:   SIL (http://scripts.sil.org/OFL)  
   Homepage:  http://somerandomdude.com/work/iconic/  
