## Feedback Button

Feedback Button adds a fixed button that opens a feedback form in a modal window. It gives students a direct way to submit comments without leaving the page.

## Customise

```js
const PAGE_CONFIGS = [{
    urlIncludes: "book/tool",
    feedback: {
        enable: true, // false
        url: "https://example.com/form"
    }
}]
```

Set `feedback.enable` to `true` to turn the feature on, or `false` to turn it off. Replace `feedback.url` with the form or survey link you want to load.

## Limitation

- The button does not appear unless both `feedback.enable` is `true` and a `feedback.url` value is provided.
- The form must allow embedding in an iframe, otherwise it may not load inside the modal.
- The current implementation is configured only in the `PAGE_CONFIGS` entry where feedback is added.
