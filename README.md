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
<style>
  air-horner {
    width: 300px;
    height: 300px;
  }
</style>
<air-horner></air-horner>
```

### Can I horn without the user interaction?
Yes. The element exposes a couple of properties and methods that you can use to
interact with the `<air-horner>` element.


#### Methods

* element.`start()`
* element.`stop()`

#### Attributes 

All attributes are managed as DOM Attributes, updating the value on the object
will update it on the element and likewise from the DOM Element to the object.

* `src` &mdash; A reference to the media element that will be played.
* `loopStart` &mdash; The start point for the looping in SS.MMMM format 
* `loopEnd` &mdash; The end point for the looping in SS.MMMM format 

### Is it possible to style the airhorn?
Not yet.

### Is it possible to change the horn sound?
Yes. You can change the src attribute on the element. Note, if you want the
audio to loop you need to define a `loopStart` and `loopEnd` attribute. Finding
a good loop point is left to the reader ;)

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
<air-horner src="test/sounds/yo.mp3" loopStart="0.616" loopEnd="1.078"></air-horner>
```

By default the `airhorn.mp3` is used.

### Can you change the loop point?
Yes. By setting the `loopStart` and `loopEnd` attributes you can control where
the looping occurs. Be careful though, you need to be careful of audio clipping.

### Can it do anything else?
Not yet.