# WebStorm-WEB-66265
Minimal reproduction for https://youtrack.jetbrains.com/issue/WEB-66265

When navigating to CSS classes via Ctrl+Click or Go To Definition, WebStorm is not able to find classes that are inside layers.

This primarily affects developers navigating from .tsx (React) files to CSS (or SCSS) module files. However, the issue
can be reproduced more simply with a JS file that imports a CSS file. 


Navigating to a regular CSS class works:

![](https://github.com/Cyral/WebStorm-WEB-66265/blob/main/first.png?raw=true)

Navigating to a CSS class within an @layer does not:

![](https://github.com/Cyral/WebStorm-WEB-66265/blob/main/second.png?raw=true)
