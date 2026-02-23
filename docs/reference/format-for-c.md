# Format for C

**Format Selection for C (MSQL Only)** is a productivity tool that converts a selected block of MOCA/MSQL code into a C-compatible `sprintf` string.

## Accessing the Feature

1. Select the MOCA/MSQL code you want to convert in the editor.
2. Go to **Edit → Format Selection for C (MSQL Only)**.

## What It Does

The conversion:

- Wraps the selected code in a C string literal
- Replaces variable references with `%s` placeholders
- Appends the variable names as a comma-separated list at the end

The result is ready to paste into a C `sprintf` statement.

## Example

**Original MOCA code:**

```
select * from orders where ordnum = @ordnum and wh_id = @wh_id
```

**After "Format Selection for C":**

```c
sprintf(query, "select * from orders where ordnum = '%s' and wh_id = '%s'",
    ordnum, wh_id);
```

This eliminates the need to manually construct the C string and reduces transcription errors when embedding MOCA queries in C code.
