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
