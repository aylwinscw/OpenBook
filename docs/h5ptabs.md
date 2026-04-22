## H5P Tabs

H5P Tabs group H5P activities that share the same parent container into a tabbed layout. This helps reduce page length and lets students move between activities more easily.

## Customise

```js
const PAGE_CONFIGS = [{
    urlIncludes: "book/tool", // One pager mode
    h5pTabs: true, // false
    ...
    urlIncludes: "mod/book/view.php", // Original Moodle Book mode
    h5pTabs: true, // false
}]
```

Set `h5pTabs` to `true` to turn the feature on, or `false` to turn it off.

## Limitation

- Tabs are created from `.h5p-placeholder` elements, so the feature depends on Moodle rendering H5P activities with that markup.
- Tab labels are generated automatically as `Question 1`, `Question 2`, and so on.
- The script groups H5P activities by shared parent container, so mixed layouts may produce more than one tab set on the same page.
