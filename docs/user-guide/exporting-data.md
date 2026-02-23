# Exporting Data

LextEdit provides multiple ways to get data out of the results grid — from quick keyboard shortcuts to context-menu copy options that generate SQL code.

## Quick Export Shortcuts

| Action | Shortcut |
|---|---|
| Export grid to Excel | `F5` |
| Quick save results to LextEdit file | `F6` |
| Export results with options | File → Export Results... |

## Copy from the Grid

Right-clicking selected rows or cells in the results grid opens a copy menu with several options:

- **Copy as WHERE clause** — generates a SQL `WHERE` clause from the selected data
- **Copy as INSERT statement** — generates a SQL `INSERT` statement
- **Copy as CSV** — copies the selected data as comma-delimited text

These options are available based on the current selection and save significant time when building queries from existing data.

## Import Editor Data

**Tools → Import Editor Data** loads text from the editor pane into the grid. The first row is treated as the header row. This pairs well with the copy options above for code generation.

## Saving and Loading Result Files

- **File → Save Results** — saves the current grid to a LextEdit result file
- **File → Load Results** — reloads a previously saved result file into the grid
- **File → Quick Save Results (F6)** — immediately saves to the default location
