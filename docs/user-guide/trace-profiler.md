# Trace Profiler

The **TraceProfiler** is LextEdit's dedicated tool for opening and analyzing MOCA trace files. It can also load other ASCII-based log files.

## Opening the Trace Profiler

- Press **Ctrl+T** from the main LextEdit window, or click the TraceProfiler icon in the toolbar.
- The Trace Profiler can also be opened directly from the toolbar shortcut **F10** when inside the TraceProfiler window.

## Interface Overview

The TraceProfiler window is divided into two main areas:

- **Left panel** — a tree-based structure representing the interpreted trace, organized by command and sub-command
- **Right panel** — the raw ASCII log text; selecting a node in the tree highlights the corresponding text on the right

## Opening Trace Files

### From a Remote MOCA Connection

1. Press **Ctrl+O** inside the Trace Profiler to browse remote trace files.
2. The file dialog automatically sorts results in time order, with the most recent file pre-selected.
3. Multiple file types are available — even files without profile information can be opened.

### From a Local File

- Press **Ctrl+L** to open a locally saved trace file.

## Starting a Trace

From the main LextEdit window:

- **F9** — starts a MOCA server trace, using the current login name as the trace profile name
- **Ctrl+F9** — starts a trace and prompts you to enter a custom profile name

## Finding Content

Use the find toolbar inside the TraceProfiler to search both the profile (tree) and log (text) sections.

## Saving Traces Locally

Press **Ctrl+S** inside the Trace Profiler to save the currently loaded trace as a local file. LextEdit automatically compresses the file on save. Saved traces can be reopened at any time with **Ctrl+L**.

Press **F5** to reopen the current trace file name (refreshes the view if the file has been updated).

## Profile Display Options

Go to **Tools → Profile Display Options** to customize how profile entries are displayed. You can add highlighting rules — for example, applying a green background to all policy-related entries — to make important patterns easy to spot.

## Features Summary

- Easily accessed from the LextEdit toolbar
- Tree-based view for fast navigation of deep traces
- Filter by command type to reduce noise
- Customizable display rules
- Save and reload trace files locally (with automatic compression)
- Double-click SELECT statements to open them directly in an [Explain Plan](../reference/explain-plan.md) window
