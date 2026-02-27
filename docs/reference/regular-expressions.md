# Regular Expressions

LextEdit's **Find and Replace** window supports regular expressions (regex), allowing pattern-based search and replacement across files. Regex is particularly useful when making structured changes to large files where simple text replacement is not expressive enough.

## Opening Find and Replace

Press **Ctrl+F** or go to **Search &rarr; Find/Replace...**.

## Using Regular Expressions

In the Find and Replace window, enable the **Regular Expression** option to switch from literal text matching to regex mode.

With regex enabled:

- Use standard regex patterns in the **Find** field
- Use capture group references (e.g., `\1`, `\2`) in the **Replace** field to reuse matched portions of the text in the replacement
- Match complex patterns across large files quickly

## Common Use Cases

- Reformatting column lists or parameter lists. For example, transforming a comma-separated list of column names into a set of individual variable assignments.
- Finding all occurrences of a pattern across a large file, such as all references to a specific table or all command invocations with a particular argument.
- Transforming structured text into a different format, such as converting MOCA variable syntax to a different notation.
- Stripping or replacing repeated patterns in generated code, such as removing trailing whitespace from every line or normalizing quote styles.

## Navigation

| Shortcut | Action |
|---|---|
| `F3` | Find next match |
| `Shift+F3` | Find previous match |

## Tips

- The Find and Replace window is available in both the main editor and the Component Lookup window.
- Large files benefit especially from regex replacement, as it can automate changes that would take significant manual effort.
- Test your regex pattern with **Find Next** before running a replace-all operation to confirm it matches what you expect.
- Capture groups (`()`) let you isolate parts of the match for use in the replacement string, which is useful for reformatting patterns while preserving their content.
