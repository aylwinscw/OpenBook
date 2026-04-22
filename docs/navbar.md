## Navigation Bar

Navigation Bar creates a fixed top navigation based on the Moodle Book table of contents. Students can jump to sections quickly, and the active section updates as they scroll.

## Customise

```js
const PAGE_CONFIGS = [{
    urlIncludes: "book/tool", // One pager mode
    navBar: true, // false
}]
```

Set `navBar` to `true` to turn the feature on, or `false` to turn it off.

## Limitation

- This feature relies on the Moodle Book table of contents being present in the expected location.
- It is currently implemented for the one-page layout in `book/tool`.
- The original table of contents list is hidden after the custom navigation bar is built.
