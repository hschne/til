---
title: StimulusJS Keyboard Event Filters
date: 2025-10-14
tags: [ruby, stimulus]
---

TIL StimulusJS supports [keyboard event filters](https://stimulus.hotwired.dev/reference/actions#keyboardevent-filter) out of the box. 

```html
<div data-controller="modal"
     data-action="keydown.esc->modal#close" tabindex="0">
</div>
```

