# Exporting Data

LextEdit provides multiple ways to get data out of the results grid, from quick keyboard shortcuts to context-menu copy options that generate SQL code. These options are designed to support downstream workflows such as building follow-up queries, loading data into other tools, or sharing results with colleagues.

## Quick Export Shortcuts

| Action | Shortcut |
|---|---|
| Export grid to Excel | `F5` |
| Quick save results to LextEdit file | `F6` |
| Export results with options | File &rarr; Export Results... |

Pressing **F5** opens a Save dialog and writes the current grid contents to an Excel spreadsheet. This is the fastest way to share query results with users who need to work with the data in a spreadsheet environment.

Pressing **F6** saves results to a LextEdit-format file in a default location without prompting. This is useful for quickly archiving a result set without interrupting your workflow. Saved files can be reloaded later with **File &rarr; Load Results**.

## Copy from the Grid

Right-clicking selected rows or cells in the results grid opens a copy menu with several options:

- **Copy as WHERE clause**: generates a SQL `WHERE` clause from the selected data. For example, selecting a row with `ordnum = 12345` and `wh_id = WH1` will generate `WHERE ordnum = '12345' AND wh_id = 'WH1'`. This is useful when you want to use query results as filters in a follow-up command.
- **Copy as INSERT statement**: generates a SQL `INSERT` statement from the selected data. Useful for constructing insert scripts from live data.
- **Copy as CSV**: copies the selected data as comma-delimited text, ready to paste into a spreadsheet or another application.

These options are available based on the current selection and can save significant time when building queries from existing data.

## Import Editor Data

**Tools &rarr; Import Editor Data** loads text from the editor pane into the grid. The first row is treated as the header row. This pairs well with the copy options above for code generation. For example, paste a set of data values into the editor, import them into the grid, then right-click to generate INSERT statements for each row.

## Saving and Loading Result Files

- **File &rarr; Save Results**: saves the current grid to a LextEdit result file
- **File &rarr; Load Results**: reloads a previously saved result file into the grid
- **File &rarr; Quick Save Results (F6)**: immediately saves to the default location

Result files are saved in a LextEdit-native format and can be reloaded into the grid at any time without re-executing the original query. This is useful for preserving snapshots of data for comparison or documentation purposes.
