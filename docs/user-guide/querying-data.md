# Querying Data

LextEdit allows you to execute SQL and MOCA commands directly from the editor and view the results in an interactive grid.

## Executing Commands

| Action | Shortcut |
|---|---|
| Execute current context | `Ctrl+Enter` |
| Execute selection only | `Ctrl+Shift+Enter` |
| Execute entire script | `Ctrl+Alt+Enter` |
| Execute with rollback | File → Execute With Rollback |
| Cancel execution | File → Cancel |

## The Results Grid

After a command executes, results appear in the grid below the editor. The grid displays:

- Column headers
- All returned rows
- Row count and elapsed time in the status area

## Transaction Control

For connections that support transactions:

- **AutoCommit** — Tools → AutoCommit (toggle)
- **Commit** — Tools → Commit
- **Rollback** — Tools → Rollback

## Saving and Loading Results

- **Save Results** — File → Save Results
- **Quick Save Results** — `F6`
- **Load Results** — File → Load Results — reloads a previously saved result set into the grid

## InteliPrompt

When connected to a MOCA system, InteliPrompt automatically suggests command names, functions, tables, columns, and indexes as you type. This reduces errors and speeds up authoring.

## Explain Plan

Press **Ctrl+E** with a query selected to open the Explain Plan window. This analyzes the query and shows join structure in a tree view, with an optional data grid below. A MOCA connection is required.

See [Explain Plan](../reference/explain-plan.md) in Reference for details.
