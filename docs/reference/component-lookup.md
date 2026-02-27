# Component Lookup

The **Component Lookup** window is a dedicated tool for browsing and inspecting MOCA commands. It is available when connected to a MOCA system and provides a live view of the commands available in that environment.

## Opening Component Lookup

Press **Ctrl+L** or go to **View &rarr; Component Lookup**.

## Searching for Commands

Type in the **Command Name** field. InteliPrompt automatically filters the list of available commands as you type, showing command name, component level, and description (if populated). This makes it easy to locate a command even when you only know part of its name.

## Viewing a Command

Select a command from the list to display:

- **Component Level**: the level in the MOCA component hierarchy
- **Type**: Local Syntax or C Function
- **Syntax**: the command text in the main text window
- **Input Arguments**: a grid listing the input parameters for the command

Understanding the input arguments is essential before calling a command from your own scripts, as MOCA commands often require specific argument names and types to execute correctly.

### Local Syntax Commands

- Can be formatted with **Ctrl+Alt+F** to improve readability
- Right-click in the main text window and select **Open Command File** to load the corresponding source file in LextEdit. This opens the file in the main editor, allowing you to read and modify the command's implementation directly.

### C Function Commands

- If the C source file is available, it is displayed in the text window. This is useful when you need to understand the low-level behavior of a built-in command.

## Shortcuts

| Shortcut | Action |
|---|---|
| `Ctrl+D` | Look up the selected text as a command name |
| `Ctrl+Alt+F` | Format the command in the Component Lookup window |
| `Ctrl+F` | Open Find and Replace in the Component Lookup window |
