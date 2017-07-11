# Scalable and Modular Architecture for CSS

## Layout rules

- [ ] CSS, by its very nature, is used to **lay elements out on the page**.
- [ ] The minor components-such as a callout, or login form, or a navigation item-sit within the scope of major components such as a header or footer.
- [ ] The major components are referred to as Layout styles.

- [ ] Major layout styles such as header and footer are traditionally styled using ID selectors but take the time to think about the elements that are common across all components of the page and use class selectors where appropriate.

- [ ] Generally, a Layout style only has **a single selector**: a single or class name.
- [ ] However, there are times that a Layout needs to respond to different factors. For example, you may have different layouts based on user preference. This layout preference would still be declared as a Layout style and used in combination with other Layout styles.
```CSS
#article {
    float: left;
}
#sidebar {
    float: right;
}
.l-flipped #article {
    float: right;
}
.l-flipped #sidebar {
    float: left;
}
```

- [ ] Layout styles are the **only** primary category type to use ID selectors.
### Using ID selectors
- [ ] To be clear, using ID attributes in your HTMl can be a good thing and in some cases, absolutely necessary. For example they provide efficient hooks for JavaScript. For CSS, however, ID selectors aren't necessary as the performance difference between ID and class selectors are nearly non-existence and can make styling more complicated due to increasing specificity.
