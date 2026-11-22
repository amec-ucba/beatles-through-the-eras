# 📄 The Beatles Through the Eras

## 🎯 Overview

Lay out and style a three-page guide to the Beatles on your own, and show what you've learned
about Flexbox, CSS Grid, responsive design, and CSS variables.

The HTML for three pages is already written:

- **Home** (`index.html`), with a hero, a card for each of the four Beatles, and a card for
  each of the band's three eras
- **Eras** (`eras.html`), with a section for each era: its name and years, an image, a few
  paragraphs, and a list of key moments
- **Albums** (`albums/index.html`), with a card for each of the band's 13 albums

`wireframes.pdf` shows the layout of each page on a phone and on a computer. Your job is to
write **all** of the CSS in `css/styles.css` so each page matches its wireframes. The wireframes
only set the layout. The colors, fonts, spacing, and overall look are your design.

This is an **independent** assignment. There is no follow-along video. After you submit, a
walkthrough video unlocks in Canvas so you can compare your work with mine. You have two weeks,
so start in the first week.

### 🧠 What You'll Show

- Lay out a header, a hero, and rows of cards with Flexbox
- Lay out a page section with CSS Grid and `grid-template-areas`, and a card grid with
  `repeat(auto-fit, minmax())`
- Write mobile-first CSS: phone styles first, then a `min-width` media query for wider screens
- Store your colors, fonts, and spacing in CSS variables, and use them everywhere
- Design a site with readable type, colors that pass contrast, and consistent spacing

## 📋 Requirements

### Flexbox

- [ ] The header puts the site name and the navigation in a column on phones and in one row on
      wider screens, with the name on the left and the nav on the right
- [ ] The nav links sit in a row, without bullets
- [ ] On Home, the hero stacks the text above the photo on phones and puts them side by side
      on wider screens
- [ ] On Home, the member cards and the era cards are rows of cards that wrap onto new lines
      as the screen gets narrower
- [ ] Space between flex items uses `gap`, not margins

### CSS Grid

- [ ] On Eras, each era (`.era`) is a grid that uses `grid-template-areas`
- [ ] On phones, each era is one column: the name, the image, the text, then the key moments
- [ ] On wider screens, the image is on the left and spans two rows, with the text and the key
      moments stacked on the right
- [ ] On Albums, the cards are in a grid that uses `repeat(auto-fit, minmax())`, so the number
      of columns changes with the screen width without a media query

### Mobile-first media query

- [ ] Your base styles, outside any media query, are for phones
- [ ] At least one `min-width` media query changes the layout for wider screens
- [ ] Every page matches its phone wireframe at about 375px and its desktop wireframe at about
      1024px
- [ ] Nothing scrolls sideways at any width

### Design

- [ ] Your fonts are set with `font-family` and end with a fallback. Google Fonts are optional.
- [ ] Headings, body text, captions, and labels have a clear size scale in `rem`
- [ ] Text colors pass a contrast check against their backgrounds
- [ ] Spacing is consistent from section to section and card to card
- [ ] The current page is highlighted in the nav (the link with the `current` class)

### CSS variables

- [ ] Colors, fonts, and spacing are stored as custom properties on `:root`
- [ ] Your rules use `var()` for those values instead of repeating them

### Stylesheet

- [ ] All of your CSS is in `css/styles.css`, and all three pages use it
- [ ] You didn't change the HTML, except to add Google Fonts `link` elements where each page's
      comment says to
- [ ] The CSS passes the [W3C CSS Validator](https://jigsaw.w3.org/css-validator/#validate_by_input)
      with no errors

### ✅ Before You Submit

Check the following:

- [ ] In DevTools device mode, every page matches its wireframes at phone and desktop widths
- [ ] You dragged the window from narrow to wide, and nothing overlaps or scrolls sideways
- [ ] Every image shows up, including on the Albums page, which is one folder down
- [ ] You did not rename or move any of the starter files
- [ ] You saved all of your files
- [ ] The site is live on GitHub Pages and the URL is in your pull request

## 📂 Starter Files

| File / Folder | Purpose |
| --- | --- |
| `index.html` | Home: the hero, the member cards, and the era cards |
| `eras.html` | Eras: one `article` for each of the three eras |
| `albums/index.html` | Albums: one `article` for each album, one folder down |
| `css/styles.css` | Empty. Write all of your CSS here. |
| `images/` | The hero and era photos, the four member portraits in `members/`, and the album covers in `albums/` |
| `wireframes.pdf` | The layout of each page on a phone (375px) and a computer (1024px) |

The HTML has only a few classes, used where the same style repeats or where no element selector
can reach. Use element and descendant selectors for everything else (for example, `header nav a`
or `.era aside`).

| Class | Where |
| --- | --- |
| `.current` | The nav link for the page you're on |
| `.hero` | The hero section on Home |
| `.cards`, `.card`, `.role` | The rows of cards on Home, each card, and the line under each card's name |
| `.era` | Each era on the Eras page |
| `.album-grid`, `.album` | The grid of albums and each album card |

## 🧮 Grading

| Criteria | What earns full credit | Points |
| --- | --- | --- |
| **Flexbox** | The header, nav, hero, and both rows of cards match the wireframes at both widths; cards wrap; spacing uses `gap`. | 18 |
| **CSS Grid** | Each era uses `grid-template-areas` and matches the wireframes at both widths, with the image spanning two rows on wider screens; the album grid uses `repeat(auto-fit, minmax())`. | 18 |
| **Mobile-first media query** | Base styles are for phones; at least one `min-width` query changes the layout; every page matches its wireframes and nothing scrolls sideways. | 18 |
| **Design** | Readable fonts with fallbacks; a clear `rem` type scale; colors that pass contrast; consistent spacing; the current page shows in the nav. | 16 |
| **CSS variables** | Colors, fonts, and spacing are custom properties on `:root`, used with `var()` throughout. | 11 |
| **Published and submitted** | One shared stylesheet that passes the CSS validator; GitHub Pages site is live; pull request into `main` with the live URL; PR URL submitted in Canvas. | 4 |
| **Total** |  | **85** |

## 📚 Resources

- Your CE7, CE8, CE9, and CE10 repos, which use every layout technique this assignment needs
- [CSS-Tricks: A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [CSS-Tricks: A Complete Guide to CSS Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)
- [MDN: Grid template areas](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Grid_layout/Grid_template_areas)
- [MDN: Using CSS custom properties](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Cascading_variables/Using_custom_properties)
- [Google Fonts](https://fonts.google.com/)
- [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- [W3C CSS Validation Service](https://jigsaw.w3.org/css-validator/#validate_by_input)

## 🆘 Getting Help

Ask during class or office hours, or post on the Canvas discussion board. Because this is an
independent assignment, I can point you to the right idea, but I won't write your CSS for you.

Before you ask, check these common problems:

- **None of your CSS works on the Albums page?** It's one folder down, but it already links to
  `../css/styles.css`. Check that you saved `css/styles.css` and didn't move it.
- **A grid area doesn't show up where you expect?** Every name in `grid-template-areas` has to
  match a `grid-area` exactly, and each row of the template needs the same number of columns.
- **The last album card stretches across the whole row?** Use `auto-fit` with `minmax()` on a
  grid, not `flex-wrap`.
- **The page scrolls sideways on a phone?** Something has a fixed width. Check images for
  `max-width: 100%`, and look for widths in `px` that are wider than a phone.
- **Your desktop layout shows up on phones too?** Your layout rules are outside the media
  query, or the query uses `max-width` instead of `min-width`.
- **A variable doesn't work?** Custom property names start with two dashes, and you use them
  with `var(--name)`. Check the spelling in both places.
- Did you save every file? Is every CSS rule closed with a `}` and every declaration ended with
  a `;`?

---

The AI policy and submission instructions are in the [README](../README.md).
