# Tooltip
> A tooltip is a popup that displays information related to an element when the element receives keyboard focus or the mouse hovers over it. It typically appears after a small delay and disappears when Escape is pressed or on mouse out.
~ *[Source](https://www.w3.org/TR/wai-aria-practices-1.1/#tooltip)*

## HTML
### Example snippet
```html
<a href="#" aria-describedby="tooltip" aria-controls="tooltip">Tooltip anchor</a>
<span role="tooltip" id="tooltip">Tooltip text</span>
```

### Roles
- Use `tooltip` for the element that wraps the tooltip.

### ARIA states
- Set `aria-describedby` on the element that triggers the tooltip to the ID of the tooltip container.
- Set `aria-controls` on the element that triggers the tooltip to the ID of the tooltip container.

## Keyboard
| Key | Function |
|------------------|-----------------------------------------|
| <kbd>esc</kbd> | Closes the tooltip. |

## Focus Management
*Nothing special*

## Examples
- [Frend](https://frend.co/components/tooltip/)
- [eBay MIND Patterns](http://ianmcburnie.github.io/mindpatterns/disclosure/tooltip/index.html)
- [OAA Accessibility](http://www.oaa-accessibility.org/example/39/)
