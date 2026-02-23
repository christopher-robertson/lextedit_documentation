# Regular Expressions

LextEdit's **Find and Replace** window supports regular expressions (regex), allowing pattern-based search and replacement across files.

## Opening Find and Replace

Press **Ctrl+F** or go to **Search → Find/Replace...**.

## Using Regular Expressions

In the Find and Replace window, enable the **Regular Expression** option to switch from literal text matching to regex mode.

With regex enabled:

- Use standard regex patterns in the **Find** field
- Use capture group references (e.g., `\1`, `\2`) in the **Replace** field
- Match complex patterns across large files quickly

## Common Use Cases

- Reformatting column lists or parameter lists
- Finding all occurrences of a pattern across a large file
- Transforming structured text into a different format
- Stripping or replacing repeated patterns in generated code

## Navigation

| Shortcut | Action |
|---|---|
| `F3` | Find next match |
| `Shift+F3` | Find previous match |

## Tips

- The Find and Replace window is available in both the main editor and the Component Lookup window.
- Large files benefit especially from regex replacement, as it can automate changes that would take significant manual effort.
