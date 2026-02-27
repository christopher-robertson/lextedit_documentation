# Custom Commands

LextEdit allows you to create a personal library of commands that can be executed with a single click from a dedicated menu in the main window. Custom Commands are useful for frequently used queries, maintenance scripts, or multi-step procedures that you want to run repeatedly without retyping them.

## Accessing Custom Commands

Go to **View &rarr; Preferences (Ctrl+P)** and select the **Custom Commands** tab.

## Creating a Command

1. In the Preferences window, navigate to the **Custom Commands** tab.
2. Right-click in the Custom Commands tree on the right side of the window.
3. Select **Add Command**.
4. Enter a name and the command text.

The command text can be any SQL or MOCA command, including multi-line scripts. Once saved, the command appears in the **Custom Commands** menu in the main LextEdit menu bar.

### Commands with Arguments

Custom commands can be configured to accept input arguments. When the command is executed, a pop-up window prompts the user to enter the required values before execution. This makes it possible to create parameterized commands that work across different records or contexts. For example, a custom command might accept a warehouse ID and an order number as arguments, and construct the appropriate MOCA command from those inputs.

## Organizing Commands

Commands can be grouped into **directories** (folders) within the Custom Commands tree to keep related commands together and make them easier to find. For example, you might group all inventory-related commands under an "Inventory" folder and all order-related commands under an "Orders" folder.

Right-click in the tree and select **Add Directory** to create a group.

## Running Custom Commands

Once created, a **Custom Commands** menu item appears in the main LextEdit menu bar. All defined commands are listed in the dropdown and can be executed directly from there. If a command has defined arguments, a prompt appears before execution to collect the required values.

Custom Commands persist across LextEdit sessions, so once set up, they are always available as long as you are using the same LextEdit installation.
