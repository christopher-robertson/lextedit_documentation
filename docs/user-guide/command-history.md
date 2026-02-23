# Command History

LextEdit automatically records every command you execute. The Command History window lets you search, browse, and navigate your full execution history.

## Opening Command History

Press **Ctrl+H** or go to **View → History Info** to open the History Navigation window.

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

## Navigating History

### Quick Navigation (Without Opening the Window)

Press **Ctrl+Alt+Up** or **Ctrl+Alt+Down** to scroll through recent history items directly in the editor without opening the History window.

### History Navigation Window

The History window provides:

- **Search** — filter history by command content, row result, status, connection string, or connection type
- **Directories tab** — shows the History folder and any sub-folders; sub-folders are unchecked by default for faster searching of recent files
- **Calendar view** — highlights days where commands were executed
- **Frequency graph** — shows the number of commands executed per hour
- **Sessions panel** — lists sessions tied to the graph; double-click a session to jump back to it in the History Navigation view
