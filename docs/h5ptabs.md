## H5P Tabs

H5P Tabs allow you to combine multiple H5P activities on the same page into multiple tabs to reduce the length of the page.

```js
const PAGE_CONFIGS = [{
    urlIncludes: "book/tool", // One pager mode
    h5pTabs: true, // false
    ...
    urlIncludes: "mod/book/view.php", // Original Moodle Book mode
    h5pTabs: true, // false
}]
```