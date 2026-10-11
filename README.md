# Star of the Moment — free embeddable widget

Give a date, a time and a place. The widget computes the real star that was closest to directly overhead at that moment — the same astronomy that powers [astarnamed.com](https://astarnamed.com).

It was built for memorial pages: someone you lost, a person or a pet, and a real star to look up at. It works for any moment you want to remember.

**Live demo** — the hosted widget is at **https://astarnamed.com/embed/death-sky**, and this repo has a [GitHub Pages demo](https://dominiclifuchun-cell.github.io/star-widget/).

## Use it in one line (recommended)

```html
<iframe src="https://astarnamed.com/embed/death-sky" style="width:100%;max-width:560px;height:640px;border:0" title="Star of the moment"></iframe>
```

The hosted version is always up to date, English/Chinese by browser language.

## Or self-host the single file

`star-widget.html` is the whole widget: one file, no build step, no dependencies, no cookies, no tracking. Save it to your site and it works.

It calls two public endpoints on astarnamed.com — `/api/birth-star/geocode` for place search and `/api/memorial/preview` for the computation. Those are the only external requests; both are free, no key required. Please don't hammer them.

## The honesty note

The widget includes a line of copy that matters: the star is real, and the name is a memorial — commercial naming is not recognized by the International Astronomical Union. Please keep that note, and keep the "Powered by A Star Named" link if you self-host. That's the deal for a free widget.

## What it computes

The point directly overhead at the given moment, then the nearest real star in the HYG catalogue (about 108,000 stars merged from the Hipparcos, Gliese and Yale surveys). Same inputs, same star, every time. The coordinates can be checked in any sky app.

## License

MIT — see [LICENSE](LICENSE). Keep the in-widget attribution when self-hosting.

---

Maintained by [A Star Named](https://astarnamed.com). `star-widget.html` mirrors our production build; Issues welcome.
