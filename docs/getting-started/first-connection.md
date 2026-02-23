# First Connection

LextEdit supports two types of connections:

- **MOCA / MSQL** — connects to a MOCA-based logistics or warehouse management system
- **ODBC** — connects to any ODBC data source, including SQL Server, MySQL, Microsoft Excel, and Access

## Opening the Connection Window

Press **F8** or go to **File → Connect** to open the Connection Information window.

## MOCA / MSQL Connection

1. In the Connection Information window, select the **Moca Servers** tab.
2. Enter the **IP address or DNS name** of the server.
3. Enter the **port number**.
4. Enter your **username** and **password**.
5. Click **Connect**.

## ODBC Connection

1. In the Connection Information window, select the **ODBC** tab.
2. Select or enter the **ODBC driver** for your data source.
3. Provide the **server/file path**, **catalog/database name**, **username**, and **password** as required.
4. Click **Connect**.

## Secured Connections

LextEdit supports exporting and importing password-protected connection configurations. This allows an administrator to create a connection, lock it with a security phrase, and distribute it to team members without exposing editable credentials.

To secure a connection:

1. After creating a connection, double-click the **open lock icon** next to the Configuration Name field.
2. Enter a security phrase and confirm it.
3. The connection is now encrypted and locked against modification.

See [Connections](../user-guide/connections.md) in the User Guide for full details.

## Disconnecting

Go to **File → Disconnect** to close the active connection.
