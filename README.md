# Bootstrap

A single-page Bootstrap 5.3.3 practice page. Everything is in `index.html`, with one image, `Picture1.jpg`.

## What's on the page

- A responsive navbar with a collapsing menu, a dropdown, a disabled link and a search form
- Several `container-lg` sections with different background utilities (`bg-danger-subtle`, `bg-info-subtle`, `bg-light`, `bg-dark-subtle`)
- Rows with `col-md-6 col-lg-10` and `col-md-6 col-lg-2` columns of placeholder text
- Card layouts using `Picture1.jpg`; one card is fixed-width (`18rem`) and its button links out to a YouTube video

There's an HTML comment in the file, left from the commit "Added comments".

## Stack

HTML and Bootstrap 5.3.3 (CSS and JS bundle), loaded from the jsDelivr CDN. No build step, no package.json, no custom CSS or JavaScript. You need to be online for the styles to load.

## Running it

Image paths are absolute (`/Picture1.jpg`), so opening `index.html` straight from disk will not show the image. Serve the folder from its root instead, for example:

```
python3 -m http.server
```

then open http://localhost:8000.

## Notes

- The Bootstrap `<script>` tag is repeated several times inside the page body, once per section. One tag at the end of `<body>` is enough.
- The first two card blocks are bare `col-4` divs outside a `row`, and none of the images have real alt text (`alt="..."`).
