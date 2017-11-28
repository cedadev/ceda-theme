# ceda-theme

This package provides the base CSS, Javascript and images for CEDA websites.

Bootswatch theme "flatly" is used as the inital bootstrap theme via CDN:

https://bootswatch.com/flatly/

The stylesheet `bootstrap.min.css` was downloaded from the above site and modified using sed to change the supplied blue color (#2c3e50) to match the CEDA blue (#092d61): 

```
wget https://maxcdn.bootstrapcdn.com/bootswatch/3.3.7/flatly/bootstrap.min.css
sed 's/2c3e50/092d61/g' bootstrap.min.css
```


JS is used from central Bootstrap CDN

js: https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js

Startbootstrap layout theme "modern-business" is used as the basis for examples
in ceda-theme-examples
https://github.com/cedadev/ceda-theme-examples

Customisations for CEDA theme are in css/ceda.css, including
* logo in navbar
https://startbootstrap.com/template-overviews/logo-nav/

Note: this theme is used in conjunction with `ceda-theme-django` to provide
styling for django apps. It is a submodule of `ceda-theme-django`