# Craftorea i18n

Centralized internationalization (i18n) translation files for the Craftorea monorepo.

## Overview

This directory contains the source of truth for all translation strings used across the Craftorea applications. The translations are organized by language and follow a nested JSON structure compatible with [next-intl](https://next-intl-docs.vercel.app/).

## Supported Languages

- **Slovak (sk)** - Primary language (`sk.json`)
- **English (en)** - Secondary language (`en.json`)
- **German (de)** - Tertiary language (`de.json`)

## Structure

Each language file (`sk.json`, `en.json`, `de.json`) contains a hierarchical JSON structure with nested keys for organizing translations by feature or component:

```json
{
  "general": {
    "apply": "Apply",
    "cancel": "Cancel",
    ...
  },
  "contact_us": {
    "title": "Contact",
    "shop": "Shop",
    ...
  }
}
```

## Best Practices

1. **Consistency**: Keep translation keys consistent across all language files
2. **Completeness**: When adding a new translation key, ensure it exists in all language files
3. **Structure**: Maintain the same nested structure across all language files
4. **Keys**: Use descriptive, hierarchical keys (e.g., `general.buttons.save` instead of `saveButton`)
5. **Placeholders**: Use clear placeholder names for dynamic content (e.g., `{name}`, `{count}`)

## Adding New Translations

1. Add the new key to all language files (`sk.json`, `en.json`, `de.json`)
2. Maintain the same JSON structure across all files
3. Ensure translations are contextually appropriate for each language
4. Test the translations in the respective applications
