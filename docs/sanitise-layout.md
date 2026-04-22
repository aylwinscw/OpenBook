## Sanitise Layout Classes

Sanitise Layout Classes removes selected Bootstrap-style layout classes from Moodle content. This can help clean up imported layouts so the book follows a more consistent single-column presentation.

## Customise

```js
const PAGE_CONFIGS = [{
    urlIncludes: "book/tool",
    sanitizeSelectors: {
        parent: ".pb-5",
        selectors: [
            ".atto_bsgrid.container-fluid",
            ".row-fluid",
            ".col-md-8",
            ".col-md-4",
            ".col-md-6",
            ".col-md-1"
        ]
    }
}]
```

To turn this behaviour on, include a `sanitizeSelectors` object with a parent selector and the classes you want removed. To turn it off, remove the `sanitizeSelectors` block from that page configuration.

## Limitation

- This feature removes classes only; it does not rebuild the original layout structure.
- It works only within the parent container you define.
- Incorrect selector choices may remove classes needed for intentional layouts.
