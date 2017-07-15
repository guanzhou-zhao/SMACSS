# Scalable and Modular Architecture for CSS

## Formatting Code

- [ ] Everyone has their own way.

#### Multiple lines

```css
.module {
  display: block;
  height: 200px;
  width: 200px;
  float: left;
  position: relative;

  border: 1px solid #333;
  -moz-border-radius: 10px;
  -webkit-border-radius: 10px;
  border-radius: 10px;

  -moz-box-shadow: 10px 10px 5px #888;
  -webkit-box-shadow: 10px 10px 5px #888;
  box-shadow: 10px 10px 5px #888;

  font-size: 12px;
  text-transform: uppercase;
}
```

  - Opening bracket on the same line as the rule set
  - one space after the colon
  - Four spaces before each declaration
  - properties are grouped by type
  - colour declarations use the short form

#### grouping properties

  1. Box
  2. Border
  3. Background
  4. Text
  5. Other

  - Box includes any property that affects the display and position of the box such as `display`, `float`, `position`, `left`, `top`, `height`, `width` and so on. These are most important because they affect the flow of the rest of the document.

  - Border includes `border`, the oft-unused `border-image` and `border-radius`.

  - Background comes next. With the advent of CSS3 gradients, background declarations can actually become quite verbose.  Once again, vendor prefixes just compound the issue.

>Multiple backgrounds with CSS3 declarations

```css
  background-color: #6d695c;
  background-image: url("/img/argyle.png");
  background-image:
  repeating-linear-gradient(-30deg, rgba(255,255,255,.1), rgba(255,255,255,.1) 1px, transparent 1px, transparent 60px), repeating-linear-gradient(30deg, rgba(255,255,255,.1), rgba(255,255,255,.1) 1px, transparent 1px, transparent 60px), linear-gradient(30deg, rgba(0,0,0,.1) 25%, transparent 25%, transparent 75%, rgba(0,0,0,.1) 75%, rgba(0,0,0,.1)), linear-gradient(-30deg, rgba(0,0,0,.1) 25%, transparent 25%, transparent 75%, rgba(0,0,0,.1) 75%, rgba(0,0,0,.1));
  background-size: 70px 120px;
```

- Text declarations include `font-family`, `font-size`, `text-transform`, `letter-spacing`, and any other CSS properties that affect the display of the type.

- Anything that doesn't fall into any of the above categories gets added to the end.

#### Colour declaration use `#000`, `#FFF`.

#### Be consistent

- [ ] The important part-like much of what SMACSS describes-is to establish a standard, document it, and be consistent with it.
