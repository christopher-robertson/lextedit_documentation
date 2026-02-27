# Querying Data

LextEdit allows you to execute SQL and MOCA commands directly from the editor and view the results in an interactive grid. Queries can be run against any active connection, whether MOCA/MSQL or ODBC.

## Executing Commands

| Action | Shortcut |
|---|---|
| Execute current context | `Ctrl+Enter` |
| Execute selection only | `Ctrl+Shift+Enter` |
| Execute entire script | `Ctrl+Alt+Enter` |
| Execute with rollback | File &rarr; Execute With Rollback |
| Cancel execution | File &rarr; Cancel |

LextEdit determines the context boundary for `Ctrl+Enter` based on the cursor position relative to blank lines and command separators. This makes it practical to keep multiple commands in a single file and execute each one individually by positioning the cursor within it.

## The Results Grid

After a command executes, results appear in the grid below the editor. The grid displays:

- Column headers
- All returned rows
- Row count and elapsed time in the status area

The grid is interactive. You can sort results by clicking a column header, resize columns by dragging column dividers, and right-click rows to access copy options. For large result sets, the grid handles many thousands of rows without a noticeable slowdown.

## Transaction Control

For connections that support transactions:

- **AutoCommit**: Tools &rarr; AutoCommit (toggle). When AutoCommit is enabled, each command is committed immediately after execution. When disabled, changes are held in an open transaction until you manually commit or roll back.
- **Commit**: Tools &rarr; Commit
- **Rollback**: Tools &rarr; Rollback

Transaction control is useful during development and testing when you want to verify the effects of a command before permanently committing changes to the database.

## Saving and Loading Results

- **Save Results**: File &rarr; Save Results
- **Quick Save Results**: `F6`
- **Load Results**: File &rarr; Load Results. Reloads a previously saved result set into the grid for review without re-executing the query.

Saved result files can be shared with colleagues or archived as a snapshot of data at a point in time.

## InteliPrompt

When connected to a MOCA system, InteliPrompt automatically suggests command names, functions, tables, columns, and indexes as you type. This reduces errors and speeds up authoring. Suggestions are drawn from the live system, so they reflect the commands and schema available in that specific environment.

## Explain Query

Press **Ctrl+E** with a query selected to open the Explain Query window. This analyzes the query and shows join structure in a tree view, with an optional data grid below. A MOCA connection is required.

Explain Query is useful for diagnosing slow queries by identifying missing indexes or inefficient join paths. It can also be launched directly from the Trace Profiler by double-clicking a SELECT statement in the trace tree.

See [Explain Query](../reference/explain-plan.md) in Reference for details.
