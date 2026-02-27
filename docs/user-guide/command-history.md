# Command History

LextEdit automatically records every command you execute. The Command History window lets you search, browse, and navigate your full execution history. This is particularly useful for reproducing a query that was run earlier, auditing what was executed during a session, or finding a previous command whose text you cannot quite recall.

## Opening Command History

Press **Ctrl+H** or go to **View &rarr; History Info** to open the History Navigation window.

## What is Recorded

Each history record contains:

- Execution status (success or error)
- Number of rows returned
- Total elapsed time
- The command text that was executed
- Start time of execution
- Row result
- Connection string used
- Connection type (MOCA/MSQL or ODBC)

History records are written to disk as individual files, organized by session and date. This means the history is persistent across LextEdit restarts and grows over time until manually cleared.

## Navigating History

### Quick Navigation (Without Opening the Window)

Press **Ctrl+Alt+Up** or **Ctrl+Alt+Down** to scroll through recent history items directly in the editor without opening the History window. The command text of each history item is loaded into the editor as you scroll, making it easy to re-run or modify a recent command.

### History Navigation Window

The History window provides:

- **Search**: filter history by command content, row result, status, connection string, or connection type. Searching by content is useful when you remember part of a command but not when it was run.
- **Directories tab**: shows the History folder and any sub-folders. Sub-folders are unchecked by default for faster searching of recent files. Uncheck older sub-folders to narrow the search scope.
- **Calendar view**: highlights days where commands were executed. Click a day to jump to the history records for that date.
- **Frequency graph**: shows the number of commands executed per hour. Useful for identifying periods of high activity during a session.
- **Sessions panel**: lists sessions tied to the graph. Double-click a session to jump back to it in the History Navigation view.
