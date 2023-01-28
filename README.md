# CSS-Reset

<h2>What is a reset and why you should use it...</h2>

<p>A CSS Reset style sheet is a list of rules that 'reset' all of the default browser styles.</p>

<p>We reset the browser styles for two primary reasons:</p>

- Not all browsers apply the same default rules. They may be similar, but not exact. It can be difficult to provide the same designs in each browser if the basic styles are different.
  - For example, a ```<button>```with no other styling whatsoever, Chrome will apply a padding: 2px 6px 3px; while Firefox applies padding: 0 8px;
- Once you start designing and coding all of the fine details of your site, you may discover that a lot of what you are doing is simply overriding default browser styles. The reset does this quickly so that you don't have to.
- This will save you a lot time and frustration when you are creating complicated layouts with CSS.
- You're the designer. You shouldn't let the browser makers decide how any part of your web pages will look.


<h2>Code Snippets</h2>

```
*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
```
```
@media (prefers-reduced-motion: reduce) {
  html:focus-within {
    scroll-behavior: auto;
  }

  *,
  *::before,
  *::after {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
    scroll-behavior: auto !important;
  }
}
```
