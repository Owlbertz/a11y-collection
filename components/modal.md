# Modals / Popups
In the W3C specs, those are referred to as **Dialogs**.
> A dialog is a window overlayed on either the primary window or another dialog window. Like non-modal dialogs, modal dialogs have their own tab sequence, i.e., Tab and Shift + Tab do not move focus outside the dialog. However, the window under a modal dialog is typically inert; users cannot interact with content outside the dialog window. So, unlike non-modal dialogs, a modal dialog does not provide means for moving keyboard focus outside the dialog window without closing the dialog.
~ *[Source](https://www.w3.org/TR/wai-aria-practices-1.1/#dialog_modal)*

## HTML
### Example snippet
```html
TODO
```

### Roles
- Use `dialog` for the container that represents the popup.

### ARIA states
- Set `aria-controls` on the popup trigger to the ID of the popup.
- Set `aria-haspopup` to `true` on the popup trigger.

## Keyboard
| Key | Function |
|------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------|
| <kbd>tab</kbd> | Moves focus to next focusable element inside the popup. If the last focusable element is focussed, the focus is moved to its first focusable element. |
| <kbd>shift + tab</kbd> | Moves focus to previous focusable element inside the popup. If the first focusable element is focussed, the focus is moved to its last focusable element. |
| <kbd>esc</kbd> | Closes the popup. |

## Focus Management
- When a popup opens, the first focusable element inside of it should receive focus.
- When a popup is closed, the focus should be reset to the element that was focussed before it has been opened. In most cases, this will be the popup trigger.
- Popups should trap the focus (see *Keyboard* section).

## Examples
- [WAI Authoring Practice](https://www.w3.org/TR/wai-aria-practices-1.1/examples/tabs/tabs.html)
- [Frend](https://frend.co/components/dialogmodal/)
