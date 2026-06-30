SilverBullet UI (Top bar, Buttons, Notifications, etc.).

# Top Bar
```space-style
/* priority: 600 */
#sb-top {
  border: none;
}
```

## Title (Top Bar)
```space-style
/* priority: 600 */
#sb-top 
{
  .sb-input {
    font-size: 1em;
    font-weight: bold;
  }
}
```

---

# Button
${widgets.button("Button", function() editor.flashNotification "Hello there 👋" end)}

```space-style
/* priority: 600 */
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
/* priority: 600 */
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
