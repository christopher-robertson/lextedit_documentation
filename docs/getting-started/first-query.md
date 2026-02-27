# First Query

Once connected to a MOCA or ODBC system, you can write and execute commands directly from the editor. LextEdit sends the command to the connected system, receives the results, and displays them in the grid below the editor.

## The Editor Window

The main LextEdit window contains a text editor pane at the top and a results grid at the bottom. Type your SQL or MOCA command in the editor, then execute it. The editor supports syntax colorization for SQL, MOCA, and many other languages, making it easy to read and write queries even in complex scripts.

## Executing a Command

LextEdit provides several execution modes depending on what you want to run:

- Press **Ctrl+Enter** to execute the current command context. LextEdit determines the boundaries of the current command based on the cursor position.
- Press **Ctrl+Shift+Enter** to execute only the selected text. This is useful when your file contains multiple commands and you want to run a specific one.
- Press **Ctrl+Alt+Enter** to execute the entire script. All commands in the file are sent as a single execution.

For a first query, try typing a simple SQL statement such as `SELECT sysdate FROM dual` (for MOCA/Oracle-based systems) and pressing **Ctrl+Enter**.

## Reading the Results

After execution, results appear in the grid below the editor. The grid shows:

- Column headers from the query result
- All returned rows
- Row count and elapsed time in the status area at the bottom of the window

You can sort the grid by clicking a column header, and resize columns by dragging the column dividers. The grid is interactive and supports copying data in multiple formats.

## Exporting Results

- Press **F5** to export the grid results to a Microsoft Excel spreadsheet.
- Press **F6** to quickly save the results in a LextEdit-based file format for later reloading.
- Right-click in the grid for additional copy options, including WHERE clause generation and INSERT statement generation. These options are especially useful for constructing follow-up queries from the returned data.

## Next Steps

- Learn about [MOCA Commands](moca-commands.md) for MOCA-specific query patterns.
- See [Querying Data](../user-guide/querying-data.md) in the User Guide for advanced query features.
- See [Exporting Data](../user-guide/exporting-data.md) for full details on copy and export options.
