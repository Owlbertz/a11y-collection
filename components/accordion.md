# Accordion
> An accordion is a vertically stacked set of elements, such as labels or thumbnails, that allow the user to toggle the display of sections of content. Each labeling element can be expanded or collapsed to reveal or hide its associated content. Accordions are commonly used to reduce the need to scroll when presenting multiple sections of content on a single page.
~ *[Source](https://www.w3.org/TR/wai-aria-practices-1.1/#accordion)*

## HTML
### Example snippet
```html
<div role="tablist">
  <h4 role="tab" aria-selected="true" id="first-accordion" aria-controls="first-accordion-panel" tabindex="0">Active panel</h4>
  <div role="tabpanel" id="first-accordion-panel" aria-labelledby="first-accordion">
    <p><a href="#">Some link inside the accordion panel.</a> Some more text inside the accordion panel.</p>
  </div>
  <h4 role="tab" aria-selected="false" id="second-accordion" aria-controls="second-accordion-panel" tabindex="0">Another panel</h4>
  <div role="tabpanel" id="second-accordion-panel" aria-labelledby="second-accordion">
    <p>This accordion panel is not active and therefore invisible.</p>
  </div>
</div>
```

### Roles
- Use `tablist` for the element that wraps the accordion.
- Use `tab` for the element that wraps the accordion title.
- Use `tabpanel` for the element that wraps the accordion panel content.

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
