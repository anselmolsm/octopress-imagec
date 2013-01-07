# Introduction

Imagec is an octpress plugin that adds a tag for image with captions.

This plugin is based on the idea posted by Aijaz Ansari on his blog[^1],
where a perl script converts a custom syntax to the a floating div tag containing an img tag plus the caption.

He proposed this syntax, processed by his perl script:
```
<!-- ai{align} {target} {image} {width} {height} {caption} -->
```

I followed the syntax for the imagec plugin:

```
{% imagec {align} {target} {image} {width} {height} "{caption}" %}
```

Notice it requires the definition of the css classes imagecc, imagecl, imagecr.

[^1]: <http://aijazansari.com/2011/12/12/switching-to-octopress/>

# Installation

* Copy `imagec.rb` to `plugins` directory at the root of you octopress repo.
* Move `style.css` into your theme's `sass/custom` directory. Notice it is just an initial definition, you can customize this style according to your needs.

# Usage

* For a centralized image, 200x200 with the amazing caption "This is a caption":
```
{% imagec c "http://asite.com" "url/to/the/image.extension" 200 200 "This is a caption" %}
```

# License

(The MIT License)

Copyright © 2012-2013 Anselmo L. S. Melo

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the ‘Software’), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED ‘AS IS’, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.