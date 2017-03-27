# Idea

[Inspiration](https://github.com/eqcss/eqcss/issues/59#issuecomment-289527014)

In the following example, all divs with "child" classes would be the same
height, if the JS runtime is included.
Could work the same way
[Container Queries](https://github.com/ZeeCoder/container-query) work:
CSS ➡ PostCSS ➡ JSON ➡ Runtime

```css
.parent {
    /* styling */
}

.child {
    @equal-height; // or some more interop declaration
}
```

```html
<div class="parent">
    <div class="child"><!-- content --></div>
    <div class="child"><!-- content --></div>
    <div class="child"><!-- content --></div>
</div>
```
