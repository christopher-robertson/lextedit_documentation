# Explain Plan

The **Explain Plan** tool analyzes SQL queries to help identify performance issues and understand how joins are being resolved.

!!! note
    A MOCA connection is required for the Explain Plan to function.

## Opening Explain Plan

- Press **Ctrl+E** with a query selected in the editor to open the Explain Plan for that query.
- From the Trace Profiler, double-click a SELECT statement to open it in an Explain Plan window.
- From the Trace Profiler toolbar, press **Ctrl+E** to open a blank Explain Plan window.

## Interface

The Explain Plan window contains three areas:

1. **Query area (top)** — shows the query being analyzed
2. **Join tree (middle)** — displays the joins in a tree structure, showing how tables are being accessed
3. **Data grid (bottom, optional)** — shows the actual data returned by the explain plan query

## Use Cases

- Identify missing indexes or inefficient join paths
- Compare execution plans before and after query changes
- Quickly analyze queries surfaced in a trace file
