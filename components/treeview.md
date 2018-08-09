# Tree View
> A tree view widget presents a hierarchical list. Any item in the hierarchy may have child items, and items that have children may be expanded or collapsed to show or hide the children. For example, in a file system navigator that uses a tree view to display folders and files, an item representing a folder can be expanded to reveal the contents of the folder, which may be files, folders, or both.
~ *[Source](https://www.w3.org/TR/wai-aria-practices-1.1/#TreeView)*

## HTML
### Example snippet
```html
<h3 id="header">Directories</h3>
<ul role="tree" aria-labelledby="header">
  <li role="treeitem" aria-expanded="true" aria-label="Folder 1 (open)" tabindex="0">
    Folder 1 (open)
    <ul role="group">
      <li role="treeitem" aria-expanded="false" aria-label="Folder 2(closed)" tabindex="-1">
        <span class="">
          Folder 2 (closed)
        </span>
        <ul role="group">
          <li role="treeitem" tabindex="-1">
            File
          </li>
        </ul>
      </li>
      <li role="treeitem" tabindex="-1">
        File
      </li>
    </ul>
  </li>  
</ul>
```

### Roles
- Use `tree` for the element that represents the tree's root.
- Use `group` for elements that contain child elements.
- Use `treeitem` for elements that serve as leaves.

### ARIA states
TODO

## Keyboard
TODO

## Focus Management
*Nothing special*

## Examples
- [WAI Authoring Practice](https://www.w3.org/TR/wai-aria-practices-1.1/examples/treeview/treeview-1/treeview-1a.html)
- [OAA Accessibility](http://www.oaa-accessibility.org/example/41/)
