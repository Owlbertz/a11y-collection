# Carousel
> [A carousel] creates a viewport around a list of items, where n items are visible at any time. We say that each viewport of items constitutes a slide.
A carousel with one item in the viewport is a Slideshow Carousel (pictured above).
A carousel with more than one item in the viewport is a Filmstrip Carousel (pictured below).
~ *[Source](https://ebay.gitbooks.io/mindpatterns/content/disclosure/carousel.html)*

## HTML
### Example snippet
```html
<button type="button" aria-label="Previous slide"></button>
<ul>
  <li>
    <div>
      <h4>First slide</h4>
    </div>
  </li>
  <li aria-hidden="true">
    <div>
      <h4>Second slide</h4>
    </div>
  </li>
</ul>
<button type="button" aria-label="Next slide"></button>
</div>
```

### Roles
*Nothing special*

### ARIA states
- Set `aria-hidden` to `true` for slides that are not visible.
- Set `aria-label` on the buttons to change slide.

## Keyboard
| Key              | Function                |
|------------------|-------------------------|
| <kbd>right</kbd> | Display next slide      |
| <kbd>left</kbd>  | Display previous slide. |

## Focus Management
*Nothing special*

## Examples
- [eBay MIND Patterns](http://ianmcburnie.github.io/mindpatterns/disclosure/carousel/index.html)
