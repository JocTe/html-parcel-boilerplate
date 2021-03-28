# This is a simple [Parcel](https://parceljs.org/) boilerplate

It uses [SASS](https://sass-lang.com/), and [posthtml-include](https://github.com/posthtml/posthtml-include).

# Partials

__locals__: Object containing any local variables that you want to be accessible inside the include component

## How to use them? 
__index.html__

```html
<html>
<head>
    <title>index.html</title>
</head>
<body>
    <include src="partials/button.html" locals='{
        "text": "Button"
    }'></include>
</body>
</html>
```

__partials/button.html__
```html
<button class="button"><div class="button__text">{{ text }}</div></button>
```