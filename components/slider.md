# Slider
> A slider is an input where the user selects a value from within a given range. Sliders typically have a slider thumb that can be moved along a bar or track to change the value of the slider.
~ *[Source](https://www.w3.org/TR/wai-aria-practices-1.1/#slider)*

## HTML
### Example snippet
```html
<div id="slider-label">Value</div>
<div id="slider" role="slider" aria-valuemin="0" aria-valuenow="10" aria-valuemax="100" aria-labelledby="slider-label" tabindex="0"></div>
```
Make sure to set `tabindex` of the element with `role="slider"` to `0` in order to make it focusable.

### Roles
- Use `slider` for the element that represents the slider thumb.

### ARIA states
- Set `aria-valuemin` to the smallest selectable value on the slider thumb.
- Set `aria-valuenow` to the current value on the slider thumb.
- Set `aria-valuemax` to the highest selectable value on the slider thumb.
- Set `aria-labelledby` on an thumb to the ID of the label that describes the slider.
- Set `aria-label` on an thumb if no other label is provided.

## Keyboard

| Key              | Function                      |
|------------------|-------------------------------|
| <kbd>right</kbd> | Increase the slider value.    |
| <kbd>up</kbd>    | Increase the slider value.    |
| <kbd>left</kbd>  | Decrease the slider value.    |
| <kbd>down</kbd>  | Decrease the slider value.    |
| <kbd>home</kbd>  | Set slider to minimum value.  |
| <kbd>end</kbd>   | Set slider to maxmimum value. |

## Focus Management
*Nothing special*

## Examples
- [WAI Authoring Practice](https://www.w3.org/TR/wai-aria-practices-1.1/examples/slider/slider-1.html)
- [OAA Accessibility](http://www.oaa-accessibility.org/examplep/slider1/)
