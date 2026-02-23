# Component Lookup

The **Component Lookup** window is a dedicated tool for browsing and inspecting MOCA commands. It is available when connected to a MOCA system.

## Opening Component Lookup

Press **Ctrl+L** or go to **View → Component Lookup**.

## Searching for Commands

Type in the **Command Name** field. InteliPrompt automatically filters the list of available commands as you type, showing command name, component level, and description (if populated).

## Viewing a Command

Select a command from the list to display:

- **Component Level** — the level in the MOCA component hierarchy
- **Type** — Local Syntax or C Function
- **Syntax** — the command text in the main text window
- **Input Arguments** — a grid listing the input parameters for the command

### Local Syntax Commands

- Can be formatted with **Ctrl+Alt+F**
- Right-click in the main text window → **Open Command File** to load the corresponding source file in LextEdit

### C Function Commands

- If the C source file is available, it is displayed in the text window

## Shortcuts

| Shortcut | Action |
|---|---|
| `Ctrl+D` | Look up the selected text as a command name |
| `Ctrl+Alt+F` | Format the command in the Component Lookup window |
| `Ctrl+F` | Open Find and Replace in the Component Lookup window |
