Style overrides for tags, code blocks, and UI elements.

# Top Bar
```space-style
/* priority: 900 */
html, body {
  --top-color: var(--text-primary);
  --top-saved-color: var(--text-primary);
  --top-unsaved-color: var(--text-secondary);
  --top-background-color: var(--surface-lower);

  --top-sync-error-color: var(--color-error);
  --top-sync-error-background-color: var(--color-error-bg);

  --action-button-hover-color: var(--accent-primary)
}

#sb-top {
  border: none;
}
```

## Title
```space-style
/* priority: 900 */

#sb-top 
{
  .cm-content {
    font-size: 1em;
    font-weight: bold;
  }
}

```

---

# Tags
Example: #linux #homelab

```space-style
/* priority: 800 */
/* Tags */
.sb-hashtag {
  color: var(--accent-primary) !important;
  background: var(--accent-primary-10) !important;
  border: 1px solid var(--accent-primary-50);
  border-radius: var(--radius-sm);
  font-family: var(--code-font) !important;
  font-size: 0.85em;
  padding: 0px 4px;
}
```

---

# Code
Use `inline code` for small code snippets.

```space-style
/* priority: 800 */
/* Inline Code */
span.sb-code {
  background: var(--editor-code-background-color) !important;
  border: 1px solid var(--code-border-subtle);
  color: var(--text-primary);
  border-radius: var(--radius-sm);
  font-family: var(--code-font) !important;
  font-size: 0.85em;
  padding: 0px 4px;
}

/* Fenced Code Blocks */
.sb-line-fenced-code {
  font-family: var(--code-font) !important;
  font-size: 0.9em !important;
  background: var(--editor-code-background-color) !important;
}

div.sb-line-fenced-code {
  padding: 0 0.8em !important;
}

/* Rounded borders */
/* First line with button */
.sb-line-fenced-code:has(.sb-actions) {
  border-top-left-radius: var(--radius-md);
  border-top-right-radius: var(--radius-md);
}

/* Last line with ``` */
.sb-line-fenced-code:has(.sb-meta):not(:has(.sb-actions)) {
  border-bottom-left-radius: var(--radius-md);
  border-bottom-right-radius: var(--radius-md);
}
```

---

# Button
${widgets.button("Button", function() editor.flashNotification "Hello there 👋" end)}

```space-style
/* priority: 800 */
.sb-lua-wrapper .sb-lua-directive-inline {
  /* Remove the default directive container styling */
  &:has(button) {
    border: none !important;
    background: transparent !important;
    padding: 0 !important;
  }

  button {
    /* Colors & Surface */
    background: var(--surface-raised);
    color: var(--text-secondary);
    border: 1px solid var(--code-border-subtle);
    
    /* Shape & Typography */
    border-radius: var(--radius-md);
    padding: 2px 10px;
    font-size: 0.85em;
    font-family: var(--editor-font);
    font-weight: 500;
    
    /* Animation */
    transition: all 0.2s ease-in-out;
    cursor: pointer;
    box-shadow: 0 1px 2px rgba(0,0,0,0.05);

    &:hover {
      background: var(--surface-hover);
      color: var(--accent-primary);
      border-color: var(--accent-primary-50);
      opacity: 1;
    }

    &:active {
      transform: translateY(1px);
      background: var(--surface-base);
    }
  }
}
```

---

# Notifications
${widgets.button("Show Message", function() editor.flashNotification "This is an message" end)}

```space-style
/* priority: 800 */
html, body {
  --notifications-background-color: var(--surface-raised);
  --notifications-border-color: var(--accent-primary);
  --notification-info-background-color: var(--surface-raised);
  --notification-error-background-color: var(--color-error-bg);
}

.sb-notifications {
  padding: 1rem 0;
}

.sb-notification-info {
  padding: .25rem !important;
  margin-bottom: .25rem !important;
  border-radius: var(--radius-md) !important;
  color: var(--accent-primary) !important;
}

.sb-notification-error {
  padding: .25rem !important;
  margin-bottom: .25rem !important;
  border-radius: var(--radius-md) !important;
  color: var(--color-error) !important;
  border-color: var(--color-error) !important;
}
```

---

# Markdown Line
```space-style
.sb-line-hr {
  border-color: var(--code-border-subtle);
}
```
