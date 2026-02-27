# MOCA Commands

MOCA (McHugh Open Component Architecture) is the command language used by many warehouse management and logistics systems. LextEdit provides first-class support for authoring and executing MOCA commands, including autocomplete, component browsing, and trace capture.

## Executing a MOCA Command

1. Ensure you are connected to a MOCA/MSQL system (see [First Connection](first-connection.md)).
2. Type your MOCA command in the editor window.
3. Press **Ctrl+Enter** to execute.

Results appear in the grid below the editor. MOCA commands follow a pipe-and-filter structure. For example:

```
list orders where wh_id = 'WH1'
 | create shipment where ordnum = @ordnum
```

Each command in the pipeline receives the results of the previous command as context. LextEdit handles multi-line and multi-command MOCA scripts and determines command context from the cursor position when you press **Ctrl+Enter**.

## InteliPrompt

When connected to a MOCA system, LextEdit's **InteliPrompt** feature provides autocomplete suggestions as you type, including MOCA command names, functions, indexes, tables, and columns. InteliPrompt is context-aware and draws its suggestions from the live system you are connected to, so the suggestions always reflect the components available in that environment.

To trigger InteliPrompt manually, begin typing a command name or field name and InteliPrompt will display matching suggestions automatically.

## Component Lookup

The **Component Lookup** window (Ctrl+L) is a dedicated tool for browsing and searching MOCA commands:

- Type a command name to filter the list using InteliPrompt.
- Select a command to view its component level, type (Local Syntax or C Function), syntax, and input arguments.
- Right-click in the text window to **Open Command File** for Local Syntax components. This opens the underlying source file directly in the LextEdit editor.
- Press **Ctrl+Alt+F** to format the component's code for easier reading.

Component Lookup is especially useful when exploring an unfamiliar system or looking up the exact argument names required by a command before writing a query.

See [Component Lookup](../reference/component-lookup.md) in Reference for more detail.

## Starting a Trace

To capture a MOCA server trace:

- Press **F9** to start a trace using the current login name as the profile name.
- Press **Ctrl+F9** to start a trace and be prompted for a custom profile name. Custom profile names make it easier to identify traces when multiple users are active on the same system.

The resulting trace file can be opened in the [Trace Profiler](../user-guide/trace-profiler.md) for detailed analysis of command execution and performance.
