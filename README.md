# Task 2

## Notes

- Began with plain (classless) semantic HTML.
- Using BEM to help with namespacing and trying to enforce a flat selector hierarchy.
- Using HTML5 https://html.spec.whatwg.org/multipage/links.html#link-type-author for author.
- Demonstrates nested grids.
- Use of Sass mixin (e.g. `visually-hidden`).
- Using comments `<!-- ... -->` to [close down inline-block spacing](https://css-tricks.com/fighting-the-space-between-inline-block-elements/).
- Demonstrates use of grid in HTML as well as Sass (deciding when to use one over the other is tricky).
- Using `flexbox` for equally spaced menu items (at wide).
- Omitted aria-roles as need some time to decide on these.

## Perhaps a better way?

- Having to duplicate the "More" component given mobile / wide view - would be better to revisit design. Using the correct attributes so that semantics aren't affected (`aria-hidden`, `visually-hidden`). Could use [Teleport](http://bbc.github.io/teleport/) to prevent duplication or, *even better*, revisit the design.
- CSS for JS-less nav seem a bit too clever. Might be better to use JS with progressive enhancement i.e. revisit menu design?

## TODO

- Add typography classes / mixins.
- Add appropriate fallbacks for no-flexbox support (e.g. IE8/9).
- Consider adding additional compilation for no media query support (e.g. IE8) using [sass-mq](https://github.com/sass-mq/sass-mq) or similar, or polyfill media queries.
- Add appropriate `aria-roles` and accessibility (screenreader).
- Consider adding additional data annotations / markup for improved SEO / sharing. Examples: Schema.org (`<time itemprop="datePublished" datetime="2016-01-13T12:00:40+0000">`), Twitter card, OpenGraph (`og:title`) etc.

## References

- https://github.com/necolas/idiomatic-css (Nicholas Gallagher)
- http://cssguidelin.es/ (Harry Roberts)