# SMACSS and Responsive Web Design

## Responsive web design: 

* The growth of mobile internet usage gave us the question about how to build websites that scale to different devices, the answer was responsive web design or RWD.

* RWD: Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.

* Responsive and adaptive web design are closely related, and often transposed as one in the same, responsive generally means to react quickly and positively to any change, while adaptive means to be easily modified for a new purpose or situation.

* Responsive design changes based of different factors like **viewport width**, while adaptive websites are built to a greoup of preset factors.

### Flexible layouts

* CSS3 introduced new relative length units like **vw, vh,vmin and vmax** 

* Use target ÷ context = result

Using the flexible grid formula we can take all of the fixed units of length and turn them into relative units.

```
section,
aside {
  margin: 1.858736059%; /*  10px ÷ 538px = .018587361 */
}
section {
  float: left;
  width: 63.197026%;    /* 340px ÷ 538px = .63197026 */   
}
aside {
  float: right;
  width: 29.3680297%;  /* 158px ÷ 538px = .293680297 */
}
```

### Media queries

* When the layout gets too small, or too large, text may become illegible and the layout may begin to break. In this event, media queries can be used to help build a better experience.

* You can initialize media queries using @media rule inside of an existing style sheet, importing a new style sheet using @import or by linking to a seperate style sheet, best way is to use **@media rule inside of an existing style sheet to avoid additional http requests**

* Logical operators include:
1- "and" logical operator to allow an extra condition to be added
2- "or" or a comma "," 
3- "not" to negate the query
4- "only" operator

example: 
```
@media all and (max-width: 420px) {
  section, aside {
    float: none;
    width: auto;
  }
}
```
### Mobile First Approach

* Use styles targetted for small viewports as the default style, then use media queries to add styles as viewpoer grows.

* Main reason for this approach is that a mobile user shouldnt have to load styles for desktop computer.

* It also advocates designing with the constraints of a mobile user in mind.

* Viewport meta tag is used with either height or width values, or scale or user-scalable.

### Flexible Media

* One quick way of making media scalable is with max-width: 100%;.

* It doesn't work on all media, like iframes and embedded media, it can be solved by having the parent element be relative and the media itself be absolutely positioned and 100% width.

## Floats:

* Float is a CSS positioning property

* Floats can be used to wrapping text around images or to create entire web layouts, but flexbox and grid are better.

* After you are done with float,its best to use the clear fix to stop anything unwanted from floating inside, so we use a clear:both; property in the element after the float to signal that we dont want it to float to it.

* Collapse is the height of the element becoming 0.

* Collapsing almost always needs to be dealt with to prevent strange layout and cross-browser problems. We fix it by clearing the float after the floated elements in the container but before the close of the container.

## Grids:

* Grid context:

1- Columns: we need to name it accordingly, like giving it a class of col-1-3 which means its the first column out of 3. then making them float left and then giving the specific columns width

2- Parent element will collapse to zerio height because its children are floated, so you need to clear it.

## SMACCS (Scalable and ModularArchitecture for CSS)

SMACCS is the process of organizing CSS files into specific files each with their own purposes.

* Five types of categories: Base, Layout, Module, State & Theme.

Base rules are the defaults, Layout rules divide the page into sections. Layouts hold one or more modules together, Modules are the reusable, modular parts of our design. They are the callouts, the sidebar sections, the product lists and so on, State rules are ways to describe how our modules or layouts will look when in a particular state, and Theme rules that are special for "some special event".
