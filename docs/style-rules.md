## Style Rules

Style Rules let you apply custom CSS through the `rules` object in each page configuration. This is useful for changing typography, spacing, media sizing, and other presentation details without editing the rest of the script logic.

## Customise

```js
const PAGE_CONFIGS = [{
    urlIncludes: "book/tool",
    rules: {
        ".book_chapter p, .book_chapter li": {
            fontSize: "18px",
            lineHeight: "1.5"
        },
        "img, iframe": {
            display: "block",
            marginLeft: "auto",
            marginRight: "auto",
            maxWidth: "100%"
        }
    }
}]
```

To turn a rule on, add it under `rules`. To turn it off, remove that selector block from `rules`.

## Limitation

- This feature is a styling helper rather than a stand-alone user-facing tool.
- Invalid selectors or CSS values can stop the intended styling from applying.
- Rules are injected globally for the page, so overlapping selectors can affect more content than expected.
