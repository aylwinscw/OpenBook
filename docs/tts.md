## Text-to-speech (TTS)

Text-to-speech (TTS) feature reads all text content on the page for the students. It also allows students to control what it reads using the previous/skip buttons.

## Customise

```js
const PAGE_CONFIGS = [{
    urlIncludes: "book/tool", // One pager mode
    tts: true, // false
}]
```

## Limitation

- The text-to-speech feature only works in one-page mode.
- Does not read text inside H5P or any content inside iframe.

