Global CSS resets and typography smoothing.

```space-style
/* priority: 900 */
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
  
  .sb-list-item-bullet,
  .cm-list-indent {
    font-family: var(--code-font) !important;
    display: inline-block;
    min-width: 1.5ch;
    text-align: right;
    margin-right: 0.5ch;
  }

  .sb-li-cursor {
    padding-right: 1ch; /* TODO: Spacing is still broken */
  }

  .cm-list-bullet {
    padding-right: 1ch;
  }

   .sb-task-checkbox {
    margin-right: 0.6ch;
  }
}

/* Selection highlight */
::selection {
  background: var(--accent-primary-50);
  color: var(--text-primary);
}
```
