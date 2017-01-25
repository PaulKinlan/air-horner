# Air Horner

Air horn to your hearts content.

[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/owner/my-element)

<!--
```
<custom-element-demo>
  <template>
    <link rel="import" href="air-horner.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html

<air-horner></air-horner>
```

## FAQ

### How do I include this?

There are two ways.

1. `<link rel="import" href="air-horner.html">`
2. `<script src="air-horner.js"></script>` &mdash; my preferred method.

The element name is already defined in the script as `<air-horner>`.

### How can I change the height and width?

The :host is an `inline-block` element that has a default dimensions of 100px x
100px. You can override this by specifiying your own width and height.

```html
<style>
  air-horner {
    width: 300px;
    height: 300px;
  }
</style>
<air-horner></air-horner>
```


### Is it possible to style the airhorn?
Not yet.

### Is it possible to change the horn sound?
Yes. You can change the src attribute on the element. Note, if you want the
audio to loop you need to define a `loopStart` and `loopEnd` attribute. Finding
a good loop point is left to the reader ;)

```html
<air-horner src="sounds/yo.mp3" loopStart="1.076" loopEnd="1.263"></air-horner>
```

By default the `airhorn.mp3` is used.

### Can you change the loop point?
Not yet.

### Can it do anything else?
Not yet.