# Accordion
> An accordion is a vertically stacked set of elements, such as labels or thumbnails, that allow the user to toggle the display of sections of content. Each labeling element can be expanded or collapsed to reveal or hide its associated content. Accordions are commonly used to reduce the need to scroll when presenting multiple sections of content on a single page.
~ *[Source](https://www.w3.org/TR/wai-aria-practices-1.1/#accordion)*

## HTML
### Example snippet
```html
TODO
```

### Roles
- Use `heading` for the element that wraps the accordion toggles.

### ARIA states
- Set `aria-expanded` to `true` on the accordion toggle of the active panel.
- Set `aria-controls` on an accordion toggle to the ID of the panel the toggle belongs to.
- Set `aria-disabled` to `true` on a disabled accordion toggle.
- Set `aria-labelledby` on an accordion panel to the ID of the toggle that belongs to it.

## Keyboard
| Key | Function |
|------------------|-----------------------------------------|
| <kbd>enter</kbd> | Triggers the selected accordion toggle. |
| <kbd>space</kbd> | Triggers the selected accordion toggle. |

## Focus Management
*Nothing special*

## Examples
- [WAI Authoring Practice](https://www.w3.org/TR/wai-aria-practices-1.1/examples/accordion/accordion1.html)
- [Frend](https://frend.co/components/accordion/)
- [eBay MIND Patterns](http://ianmcburnie.github.io/mindpatterns/disclosure/accordion/index.html)
- [OAA Accessibility](http://www.oaa-accessibility.org/example/35/)
