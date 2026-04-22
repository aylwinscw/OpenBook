## Learning Navigation

Learning Navigation adds quick links that let students switch between the classic Moodle Book view and the interactive one-page view. This makes it easier for students to choose the layout that suits them.

## Customise

```js
const PAGE_CONFIGS = [{
    urlIncludes: "book/tool", // One pager mode
    learnNav: true, // false
},
{
    urlIncludes: "mod/book/view.php", // Original Moodle Book mode
    learnNav: true, // false
}]
```

Set `learnNav` to `true` to turn the feature on, or `false` to turn it off.

## Limitation

- The links are built for `moodle.telt.unsw.edu.au`, so other Moodle sites need the URLs updated in the script.
- The feature depends on the `id` query parameter being present in the page URL.
- Placement differs between the one-page view and the original Moodle Book view.
