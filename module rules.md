# Scalable and Modular Architecture of CSS

## Module rules

#### A module is a more discrete component of the page

- It's your navigation bars and your carousels and your dialogs and your widgets and so on.
- Modules are the meat of the page.
- Modules sit inside Layout components.
- Modules can sometimes sit inside other modules too.
- Each module should be designed to exist as a standalone component. In doing so, the page will be more flexible.
- If doing right, modules can easily be **moved to different parts of the layout without breaking**.

#### When defining the rule set of a module

- avoid using IDs and element selectors
- sticking only to class names.
- A module wil likely contain a number of elements and there is likely to be a desire to use descendent or child selectors to target those elements.
```CSS
  .module > h2 {
  padding: 5px;
  }
  .module span {
  padding: 5px;
  }
```

##### Avoid element selectors
Styling with generic element
```html
  <div class="fld">
    <span>Folder Name</span>
  </div>
```
```CSS
  /* The Folder Module */
  .fld > span {
    padding-left: 20px;
    background: url(icon.png);
  }
```

- The problem is that as the project grows in complexity, the more likely you will need to expand a component's functionality and the more limited you will be in having used such a generic element in your rule.

Styling with generic element
```html
  <div class="fld">
    <span>Folder Name</span>
    <span>(32 items)</span>
  </div>
```

- Now we are in a pickle. We don't want the icon to appear on both elements within our folder module.

- **Only include a selector that includes semantics. A span or div holds none. A heading has some. A class defined on an element has plenty.**

Styling with generic element
```html
  <div class="fld">
    <span class="fld-name">Folder Name</span>
    <span class="fld-items">(32 items)</span>
  </div>
```
- By adding the classes to the elements, we have increased the semantics of what those elements mean and removed any ambiguity when it comes to styling them.
