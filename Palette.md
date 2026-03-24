Light and Dark mode color definitions.

```space-style
/* priority: 1000 */
html[data-theme="dark"] {
  --accent-primary: #5c7cff; /* Refined from pure blue */
  --accent-secondary: #7c89ff;
  --surface-base: #0f1115;
  --surface-lower: #090a0c;
  --surface-raised: #1c1e26;
  --surface-hover: #23262f;
  --border-default: #282a36;
  --text-primary: #f0f1f4;
  --text-secondary: #9499b0;
  --text-tertiary: #4b526d;
  
  --color-error: #f15e61;
  --color-error-bg: #3b1c1d;
  
  --editor-code-background-color: #161821;
  --code-border-subtle: #282a36;
}

html[data-theme="light"] {
  --accent-primary: #464cfc;
  --accent-secondary: #6366f1;
  --surface-base: #f8fafc;
  --surface-lower: #f1f5f9;
  --surface-raised: #e2e8f0;
  --surface-hover: #cbd5e1;
  --border-default: #e2e8f0;
  
  --text-primary: #1e293b;
  --text-secondary: #475569;
  --text-tertiary: #94a3b8;
  
  --color-error: #e7000b;
  --color-error-bg: #fde5e6;
  
  --editor-code-background-color: #f1f5f9;
  --code-border-subtle: #cbd5e1;
}

/* Computed Accent Opacities */
:root {
  --accent-primary-10: color-mix(in srgb, var(--accent-primary), transparent 90%);
  --accent-primary-50: color-mix(in srgb, var(--accent-primary), transparent 50%);
  --selection-bg: color-mix(in srgb, var(--accent-primary), transparent 70%);
}
```
