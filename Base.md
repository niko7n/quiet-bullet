Global CSS resets and typography smoothing.

```space-style
/* priority: 800 */
body {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-rendering: optimizeLegibility;
  font-variant-ligatures: discretionary-ligatures;

  /* Fix List Indentation for Proportional Fonts */
  .cm-content {
    font-family: var(--editor-font);
    font-variant-numeric: tabular-nums;
  }
}

/* Selection highlight */
::selection {
  background: var(--accent-primary-50);
  color: var(--text-primary);
}
```
