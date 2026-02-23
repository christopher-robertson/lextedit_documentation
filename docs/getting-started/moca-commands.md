# MOCA Commands

MOCA (Middleware Object-oriented Communication Architecture) is the command language used by many warehouse management and logistics systems. LextEdit provides first-class support for authoring and executing MOCA commands.

## Executing a MOCA Command

1. Ensure you are connected to a MOCA/MSQL system (see [First Connection](first-connection.md)).
2. Type your MOCA command in the editor window.
3. Press **Ctrl+Enter** to execute.

Results appear in the grid below the editor.

## InteliPrompt

When connected to a MOCA system, LextEdit's **InteliPrompt** feature provides autocomplete suggestions as you type — including MOCA command names, functions, indexes, tables, and columns.

## Component Lookup

The **Component Lookup** window (Ctrl+L) is a dedicated tool for browsing and searching MOCA commands:

- Type a command name to filter the list using InteliPrompt.
- Select a command to view its component level, type (Local Syntax or C Function), syntax, and input arguments.
- Right-click in the text window to **Open Command File** for Local Syntax components.
- Press **Ctrl+Alt+F** to format the component's code.

See [Component Lookup](../reference/component-lookup.md) in Reference for more detail.

## Starting a Trace

To capture a MOCA server trace:

- Press **F9** to start a trace using the current login name as the profile name.
- Press **Ctrl+F9** to start a trace and be prompted for a custom profile name.

The resulting trace file can be opened in the [Trace Profiler](../user-guide/trace-profiler.md).
