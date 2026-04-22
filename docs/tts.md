## Text-to-speech (TTS)

Text-to-speech (TTS) reads visible text content on the page aloud for students. It also adds previous, play or pause, and next controls so students can move through the content at their own pace.

## Customise

```js
const PAGE_CONFIGS = [{
    urlIncludes: "book/tool", // One pager mode
    tts: true, // false
}]
```

Set `tts` to `true` to turn the feature on, or `false` to turn it off.

## Limitation

- The text-to-speech feature is only enabled for page configurations where `tts` is turned on.
- It does not read content inside H5P activities, iframes, form controls, or hidden elements.
- Available voices depend on the browser and device, so the selected voice may vary between users.
