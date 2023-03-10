noscript tag escaping child elements on hydration #1601
========================================================================

GitHub Issue: https://github.com/solidjs/solid/issues/1601

```
npm install
node server
```

1. Open in the browser *with javascript disabled* and see 大丈夫 (within `<strong>` tags).
2. Disable JavaScript, and observe the error output in the console:

```
Uncaught The browser resolved template HTML does not match JSX input:
<noscript>&lt;strong&gt;大丈夫&lt;/strong&gt;</noscript>

<noscript><strong>大丈夫</strong></noscript>. Is your HTML properly formed?
```
