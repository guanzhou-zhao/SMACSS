# Scalable and Modular Architecture for CSS

## HTML5 and SMACSS

#### SMACSS has two core goals.

 - [ ] Increase the semantic value of a section of HTML and content.
 - [ ] Drease the expectation of a specific HTML structure.

#### HTML5 introduces a number of new elements

  - [ ] Tags like `section`, `header`, and `aside` are more descriptive than a simple `div`.
  - [ ] The extra tags and attributes have allowed us to be more descriptive.

#### Class names help describe our content in very specific ways-ways that are more specific than even HTML5 can provide.

```css
<nav class="l-inline">
  <h1>Primary Navigation</h1>
  <ul>
    <li>About Us
      <ul class="l-stacked">
        <li>Team</li>
        <li>Location</li>
      </ul>
    </li>
  </ul>
</nav>
```
