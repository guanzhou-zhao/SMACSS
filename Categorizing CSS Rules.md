# Scalable and Modular Architecture for CSS

## Categorizing CSS Rules

- [ ] How do you decide whether to use ID selector, or class selector or any number of  selectors that are at your disposal?
- [ ] How do you decide which elements should get the magic you wish to bestow upon it?
- [ ] How do you make it easy to understand how your site and your style are organized?

- [ ] At the very core of SMACSS is categorization.
- [ ] By categorizing CSS rules, we begin to see patterns and can define better practices around each of these patterns.

- [ ] There are five types of categories:
  * Basic
  * Layout
  * Module
  * State
  * Theme

- [ ] If we are more aware of what we are trying to style, we can avoid the complexity that comes from intertwining these rules.

- [ ] How are you going to code things? And Why are you going to code things that way?

- [ ] Much of the purpose of categorizing things is to codify patterns-things that repeat themselves within our design.
- [ ] [ ] Repetition results in less code, easier maintenance, and great consistency in the user experience.

### Base rules

- [ ] Base rules are the defaults. They are almost exclusively single element selectors but it could include attribute selectors, pseudo-class selectors, child selectors and sibling selectors. Essentially, a base style says that wherever this element is on the page, it should look like this.

### Layout rules

- [ ] Layout rules divide the pages into sections. Layouts hold one or more modules together.

### Modules

- [ ] Modules are reusable, modular parts of our design. They are the callouts, the sidebar sections, the product lists and so on.

### State rules

- [ ] State rules are the ways to describe how our modules and layouts will look when in a particular state. Is it hidden or expanded? Is it active or inactive? They are about describing how a module or layout looks on screens that are smaller or bigger. They are also about describing how a module or layout might look in different views like the home page or inside page.

### Theme rules

- [ ] Theme rules are similar to state in that they describe how a module or layout might look. Most sites don't require a layer of theming but it's good to be aware of it.

## Naming Conventions

- [ ] By separating rules into five categories, naming conventions are beneficial for immediately understanding which category a particular style belongs to and its role within the overall scope of the page.
- [ ] On larger projects, it's more likely to have styles broken up across multiple files. In these cases, naming conventions also make it easier to find which file a style belongs to.
- [ ] I like to use prefix to differentiate between Layout, State and module rules.
