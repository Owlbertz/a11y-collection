# Switch / Toggle Button
> A type of checkbox that represents on/off values, as opposed to checked/unchecked values. See related checkbox.
~ *[Source](https://www.w3.org/TR/wai-aria-1.1/#switch)*

> Toggle button: A two-state button that can be either off (not pressed) or on (pressed).
~ *[Source](https://www.w3.org/TR/wai-aria-practices/#button)*

## HTML
### Example snippet (Toggle Button)
```html
<button aria-pressed="false">
  Select
</button>
```

### Roles
*Nothing special*

### ARIA states
- Set `aria-pressed` to `true` if the toggle button is active, `false` otherwise.


## Keyboard
| Key | Function |
|------------------|----------------------------|
| <kbd>enter</kbd> | Toggles the switch/button. |
| <kbd>space</kbd> | Toggles the switch/button. |

## Focus Management
*Nothing special*

## Examples
- [WAI Authoring Practice](https://www.w3.org/TR/wai-aria-practices/examples/button/button.html)
- [Inclusive Components](https://inclusive-components.design/toggle-button/)
- [ARIA Switch Button by scottaohara](https://github.com/scottaohara/aria-switch-button)
