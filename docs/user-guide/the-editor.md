# The Editor

**LextEdit** is short for *Language Extendable Editor*. The editor is the central workspace in LextEdit, combining file editing with direct database connectivity.

## Overview

The main LextEdit window contains:

- A **text editor pane** for writing SQL, MOCA, or any supported language
- A **results grid** that displays data returned by executed commands
- A **toolbar** providing quick access to common actions

## Editor Features

### Syntax Colorization

LextEdit provides grammatical and semantic parsing with colorization for over 20 programming languages. Colorization updates on the fly as you type.

### File Operations

- **Open** — `Ctrl+O` or drag and drop a file into the editor window
- **Save** — `Ctrl+S`
- **Save As** — File → Save As...

### Text Editing

- **Undo / Redo** — standard Ctrl+Z / Ctrl+Y behavior
- **Indent / Outdent** — Edit → Indent or Outdent
- **Comment / Uncomment** — Edit → Comment Selection or Uncomment Selection
- **Uppercase (smart)** — `Ctrl+Shift+U` — uppercases selected text but preserves strings
- **Lowercase (smart)** — `Ctrl+U` — lowercases selected text but preserves strings
- **Format Code** — `Ctrl+Alt+F` — formats the current editor content

### Code Snippets

Use **Edit → Insert Code Snippet** to insert pre-defined code templates.

## Database Connectivity

When connected to a MOCA or ODBC system:

- **Execute** — `Ctrl+Enter` runs the current command context
- **Execute Selection** — `Ctrl+Shift+Enter` runs only selected text
- **Execute Script** — `Ctrl+Alt+Enter` runs the entire file contents
- **InteliPrompt** — autocomplete for MOCA commands, functions, tables, columns, and indexes

Results are displayed in the grid below the editor.

## Toolbar Access to Other Tools

From the editor toolbar you can directly open:

- **Trace Profiler** — click the TraceProfiler toolbar icon or press `Ctrl+T`
- **Component Lookup** — `Ctrl+L`
- **Explain Plan** — `Ctrl+E`
- **History** — `Ctrl+H`

## Import Editor Data

Use **Tools → Import Editor Data** to import data from the editor directly into the results grid. The first row is treated as the header row. This pairs well with the grid's copy options for code generation workflows.

## Execute with Local File

Use **Tools → Execute with Local File** to run a command against every row in a local CSV file:

1. Prepare a CSV file with the required field headers and data rows.
2. Paste the command you want to run into the editor.
3. Select **Tools → Execute with Local File**.
4. Locate and open your CSV file.
5. LextEdit shows a preview of the parsed data — confirm to proceed.
6. LextEdit executes the command for all rows in a single pass.
