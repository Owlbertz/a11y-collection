# Tabs
> Tabs are a set of layered sections of content, known as tab panels, that display one panel of content at a time. Each tab panel has an associated tab element, that when activated, displays the panel. The list of tab elements is arranged along one edge of the currently displayed panel, most commonly the top edge.
~ *[Source](https://www.w3.org/TR/wai-aria-practices-1.1/#tabpanel)*

## HTML
### Example snippet
```html
<div role="tablist">
  <button role="tab" aria-selected="true" aria-controls="first-tab-panel" id="first-tab">Active tab</button>
  <button role="tab" aria-selected="false" aria-controls="second-tab-panel" id="second-tab" tabindex="-1">Another tab</button>
</div>

<div role="tabpanel" id="first-tab-panel" aria-labelledby="first-tab">
  <p><a href="#">Some link inside the tab panel.</a> Some more text inside the tab panel.</p>
</div>

<div role="tabpanel" id="second-tab-panel" aria-labelledby="second-tab" hidden>
  <p>This tab panel is not active and therefore invisible.</p>
</div>
```
### Roles
- Use `tablist` for the container that contains the tabs.
- Use `tab` for the tab itself.
- Use `tabpanel` for the tab panel, i.e. the content belonging to a tab.

### ARIA states
- Set `aria-controls` on a tab to the ID of the panel that it belongs to.
- Set `aria-labelledby` on an tab panel to the ID of the tab that belongs to it.
- Set `aria-orientation` on an tablist-element to `vertical` for vertical tabs (`horizontal is the default`).

## Keyboard
| Key | Function |
|------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------|
| <kbd>tab</kbd> | Moves focus to first focusable element inside the active tab panel or the next one after the tabs if no focusable element inside the active tab panel. |
| <kbd>right</kbd> | Opens the next tab if focus is on any tab. |
| <kbd>left</kbd> | Opens previous tab if focus is on any tab. |

## Focus Management
- Pressing <kbd>tab</kbd> while focus is on any tab will focus the first focusable element inside the active tab panel. If no focusable element is present in the active tab panel, the tabs component is left and the next focusable element receives focus.

## Examples
- [WAI Authoring Practice](https://www.w3.org/TR/wai-aria-practices-1.1/examples/tabs/tabs.html)
- [Frend](https://frend.co/components/tabs/)
- [eBay MIND Patterns](http://ianmcburnie.github.io/mindpatterns/disclosure/tabs/index.html)
- [OAA Accessibility](http://www.oaa-accessibility.org/example/34/)
