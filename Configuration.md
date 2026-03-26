Main font stacks and layout variables.

```space-style
/* priority: 1000 */
:root {
  /* Main Fonts */
  --editor-font: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif;
  --code-font: "IBM Plex Mono", "SF Mono", Menlo, Monaco, Consolas, monospace;

  /* Border Radii */
  --radius-xs: 3px;
  --radius-sm: 4px;
  --radius-md: 6px;
  --radius-lg: 8px;
  --radius-xl: 10px;

  /* Root Mappings */
  --root-background-color: var(--surface-base);
  --root-color: var(--text-primary);
  --ui-accent-color: var(--accent-primary);

  /* Interface Mappings */
  --top-color: var(--text-primary);
  --top-saved-color: var(--text-primary);
  --top-unsaved-color: var(--text-secondary);
  --top-background-color: var(--surface-lower);
  --top-sync-error-color: var(--color-error);
  --top-sync-error-background-color: var(--color-error-bg);
  --action-button-hover-color: var(--accent-primary);

  --notifications-background-color: var(--surface-raised);
  --notifications-border-color: var(--accent-primary);
  --notification-info-background-color: var(--surface-raised);
  --notification-error-background-color: var(--color-error-bg);

  /* Editor Mappings */
  --editor-widget-background-color: var(--surface-lower);
  --editor-blockquote-background-color: var(--surface-lower);
  --editor-blockquote-border-color: var(--accent-primary);
}
```
