# CSS

## Layout

- fixed width Layouts
  - Fixed width layout designs do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels.
  - Pixel values are accurate at controlling size.
  - The designer has far greater control over the appearanceYou can control the lengths of lines of text regardless of the size of the user's window
  - The size of an image will always remain the same relative to the rest of the page.
  - You can end up with big gaps around the edge of a page.
  - If a user increases font sizes, text might not fit into the allotted spaces.
  - The design works best on devices that have a site or resolution similar to that of desktop or laptop computers.
  - The page will often take up more vertical space than a liquid layout with the same content.

```css
body {
  width: 960px;
  margin: 0 auto;
}
```

---

- Liquid Layouts
  Liquid layout designs stretch and contract as the user increases
  or decreases the size of their browser window. They tend to use percentages.
  - Pages expand to fill the entire browser window so there are no spaces around the page on a large screen.If the user has a small window, the page can contract to fit it without the user having to scroll to the side
  - If you do not control the width of sections of the page then the design can look very different than you intended, with unexpected gaps around certain elements or items squashed together.
  - If the user has a wide window, lines of text can become very long, which makes them harder to read.
  - very narrow window, words may be squashed and you can end up with few words on each line. If a fixed width item (such as an image) is in a box that is too small to hold it (because the user has made the window smaller) the image can overflow over the text.

```css
body {
  width: 90%;
  margin: 0 auto;
}
```

- Layout grids

  - Creates a continuity between different pages which may use different designs
  - Helps users predict where to find information on various pages
  - Makes it easier to add new content to the site in a consistent way
  - Helps people collaborate on the design of a site in a consistent way

- possibLe Layouts: 960 pixeL wide 12 CoLumn grid
  ![960 pixeL wide 12 CoLumn grid](https://www.sitepoint.com/wp-content/uploads/2013/05/960-12-col-grid.jpg)

---

- Css frameworKs

providing the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on.

- muLtipLe styLe sheets

`@import` `@import url("tables.css");` Your HTML page can link to one style sheet and that stylesheet can use the @import rule to import other style sheets.
