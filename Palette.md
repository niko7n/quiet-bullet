Light and Dark mode color definitions.

```space-style
/* priority: 1000 */
html[data-theme="dark"] {
  --accent-primary: #818cf8;
  --accent-secondary: #fbbf24;
  --surface-base: #0b0e14;
  --surface-lower: #11141b;
  --surface-raised: #1a1d26;
  --surface-hover: #222632;
  --border-default: #1e232e;

  --text-primary: #f1f5f9;
  --text-secondary: #94a3b8;
  --text-tertiary: #475569;
  
  --color-error: #f15e61;
  --color-error-bg: #3b1c1d;
  
  --code-border-subtle: #1e232e;
}

html[data-theme="light"] {
  --accent-primary: #464cfc;
  --accent-secondary: #ff9100;
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
  
  --code-border-subtle: #cbd5e1;
}

/* Computed Accent Opacities */
:root {
  --accent-primary-10: color-mix(in srgb, var(--accent-primary), transparent 90%);
  --accent-primary-50: color-mix(in srgb, var(--accent-primary), transparent 50%);
  --accent-secondary-10: color-mix(in srgb, var(--accent-secondary), transparent 90%);
  --accent-secondary-25: color-mix(in srgb, var(--accent-secondary), transparent 75%);
  --accent-secondary-50: color-mix(in srgb, var(--accent-secondary), transparent 50%);
  --selection-bg: color-mix(in srgb, var(--accent-primary), transparent 70%);
}
```
