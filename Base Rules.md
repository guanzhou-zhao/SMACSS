# Scalable and Modular Architecture for CSS

## Base rules
- [ ] Base rule is applied **to an element** using an element selector, a descendent selector, or a child selector, along with any pseudo-classes.
- [ ] It doesn't include any class or ID selectors.
- [ ] It is defining the default styling for how that element should look in all occurrences on the page.

- [ ] Base rules include setting heading sizes, default link styles, default font styles, and body backgrounds. there should be no need to use `!important` in a Base style.
- [ ] Highly recommended to specify a body background.

### CSS Reset

- [ ] A CSS Reset is a set of Base styles designed to strip out -or reset- the default margin, padding and other properties.
- [ ] It's purpose is to define a **consistent foundation across browsers** to build site on.

- [ ] Many reset frameworks can be overly aggressive and can introduce more problems than they solve.
- [ ] Developing **your own set of default styles** that you consistently use from project to project can also be advantageous.
