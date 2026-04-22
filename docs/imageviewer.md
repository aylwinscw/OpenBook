## Image Viewer

Image Viewer allows students to open larger images in a full-screen overlay. If an image is also linked, the script can add a separate button so students can still open the original link.

## Customise

```js
const PAGE_CONFIGS = [{
    urlIncludes: "book/tool", // One pager mode
    enableFullscreenImages: true, // false
}]
```

Set `enableFullscreenImages` to `true` to turn the feature on, or `false` to turn it off.

## Limitation
- Only images at least 100 by 100 pixels receive the full-screen control.
- Linked images are re-wrapped by the script, so unusual image markup may behave differently.
- Small decorative graphics may still be treated as images if they meet the size threshold.
