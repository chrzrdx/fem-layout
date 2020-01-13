# responsive design

- media queries
- images that resize (use `<picture>` tag)
- flexbile grid based design

# overview of floats

if you float, you must clear.

```
.row
  .col-1
  .col-1
  .col-1

.row::after
  content: ""
  display: table
  clear: both
  
.col-1:
  float: left
  margin-left: 4%
  width: 20%
```

layout problem with floats: equal sized cols so that they wrap nicely

```
[class*="col-"]
  position: relative

.col-push-1
  left: 26%

.col-push-3
  left: -74%
```

Trick with attribute selectors:

```
[href*=".pdf"]::before
  content: ""
```

you can use the above selector to add an image before each href pdf link?!

TODO: learn about floats, before/after