# First Connection

LextEdit supports two types of connections:

- **MOCA / MSQL**: connects to a MOCA-based logistics or warehouse management system using an IP address or hostname, port number, and user credentials.
- **ODBC**: connects to any ODBC data source, including SQL Server, MySQL, Microsoft Excel, and Access. ODBC connections require a driver to be pre-configured in the Windows ODBC Data Source Administrator.

## Opening the Connection Window

Press **F8** or go to **File &rarr; Connect** to open the Connection Information window.

## MOCA / MSQL Connection

1. In the Connection Information window, select the **Moca Servers** tab.
2. Enter the **IP address or DNS name** of the server.
3. Enter the **port number**.
4. Enter your **username** and **password**.
5. Click **Connect**.

Once connected, the status bar at the bottom of the main window will display the active connection details. InteliPrompt becomes available for command autocomplete.

## ODBC Connection

1. In the Connection Information window, select the **ODBC** tab.
2. Select or enter the **ODBC driver** for your data source.
3. Provide the **server/file path**, **catalog/database name**, **username**, and **password** as required by your ODBC driver.
4. Click **Connect**.

ODBC connections are useful for running SQL queries against Excel spreadsheets, Access databases, or any other ODBC-compatible system without needing a full MOCA environment.

## Secured Connections

LextEdit supports exporting and importing password-protected connection configurations. This allows an administrator to create a connection, lock it with a security phrase, and distribute it to team members without exposing editable credentials.

To secure a connection:

1. After creating a connection, double-click the **open lock icon** next to the Configuration Name field.
2. Enter a security phrase and confirm it.
3. The connection is now encrypted and locked against modification.

Secured connections can also be restricted so they can only be used with the Trace Profiler or only with the main editor. This is useful for distributing read-only or trace-specific connections to users who do not need full query access.

See [Connections](../user-guide/connections.md) in the User Guide for full details.

## Disconnecting

Go to **File &rarr; Disconnect** to close the active connection. LextEdit will continue to function as a file editor after disconnecting.
