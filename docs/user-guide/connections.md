# Connections

LextEdit supports two connection types: **MOCA/MSQL** for logistics and warehouse systems, and **ODBC** for SQL databases, Excel, and Access.

## Opening the Connection Window

Press **F8** or go to **File &rarr; Connect** to open the Connection Information window.

## Connection Types

### MOCA / MSQL

Connects to a MOCA-based server using an IP address or DNS name, port, username, and password. MOCA is the command language used by many warehouse management and logistics systems. When connected to a MOCA system, all InteliPrompt and Component Lookup features become available.

### ODBC

Connects to any configured ODBC data source. Useful for SQL Server, MySQL, Microsoft Excel, Microsoft Access, and other ODBC-compatible systems. The ODBC driver must be installed and configured in the Windows ODBC Data Source Administrator before it appears as an option in LextEdit.

## Creating a Connection

1. Open the Connection Information window (**F8**).
2. Select the appropriate tab (Moca Servers or ODBC).
3. Fill in the required fields (address, port, driver, username, password, etc.).
4. Click **Connect**.

Connection configurations are saved and can be reused. Previously created connections appear in the configuration list when you reopen the Connection Information window.

## Secured Connections

LextEdit provides a way to create encrypted, locked connection configurations. This is useful for distributing connection settings to other users without allowing them to view or modify the credentials. Secured connections are commonly used in environments where connection credentials must be tightly controlled, such as production systems.

### How to Secure a Connection

1. Create a connection as normal.
2. Double-click the **open lock icon** next to the Configuration Name field.
3. Enter and confirm a security phrase. This encrypts the connection.
4. The connection is now locked and cannot be modified without the security phrase.

### Applying Restrictions

A secured connection can be restricted to:

- **Trace Profiler Only**: the connection can only be used to open trace files
- **LextEdit Only**: the connection can only be used in the main editor

These restrictions are enforced once the connection is locked. This allows an administrator to grant trace-only access to users who should not have query access to a system.

### Exporting and Distributing Connections

Locked connection configurations can be exported and shared with other users. Recipients can use the connection without being able to view or alter the underlying settings. This makes it straightforward to standardize connection configurations across a team without risk of credential exposure.

## Changing Password

Go to **File &rarr; Change Password** to update the password for the current connection.

## Disconnecting

Go to **File &rarr; Disconnect** to close the active connection. After disconnecting, LextEdit remains fully functional as a file editor. You can reconnect to the same or a different system at any time by pressing **F8**.
