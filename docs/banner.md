## Banner

Banner adds a large welcome section at the top of the page with a gradient background and introductory text. It can be used to give the book a more course-like landing experience.

## Customise

```js
const PAGE_CONFIGS = [{
    urlIncludes: "book/tool", // One pager mode
    banner: true, // false
}]
```

Set `banner` to `true` to turn the feature on, or `false` to turn it off.

## Limitation

- The current banner text is hard-coded in the script and must be edited manually to match the course.
- The background colours are generated randomly on each page load.
- The feature does not currently pull course title, module title, or instructor details from Moodle automatically.
