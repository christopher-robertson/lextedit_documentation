# Connections

LextEdit supports two connection types: **MOCA/MSQL** for logistics and warehouse systems, and **ODBC** for SQL databases, Excel, and Access.

## Opening the Connection Window

Press **F8** or go to **File → Connect** to open the Connection Information window.

## Connection Types

### MOCA / MSQL

Connects to a MOCA-based server using an IP address or DNS name, port, username, and password.

### ODBC

Connects to any configured ODBC data source. Useful for SQL Server, MySQL, Microsoft Excel, Microsoft Access, and other ODBC-compatible systems.

## Creating a Connection

1. Open the Connection Information window (**F8**).
2. Select the appropriate tab (Moca Servers or ODBC).
3. Fill in the required fields (address, port, driver, username, password, etc.).
4. Click **Connect**.

## Secured Connections

LextEdit provides a way to create encrypted, locked connection configurations. This is useful for distributing connection settings to other users without allowing them to view or modify the credentials.

### How to Secure a Connection

1. Create a connection as normal.
2. Double-click the **open lock icon** next to the Configuration Name field.
3. Enter and confirm a security phrase — this encrypts the connection.
4. The connection is now locked and cannot be modified without the security phrase.

### Applying Restrictions

A secured connection can be restricted to:

- **Trace Profiler Only** — the connection can only be used to open trace files
- **LextEdit Only** — the connection can only be used in the main editor

These restrictions are enforced once the connection is locked.

### Exporting and Distributing Connections

Locked connection configurations can be exported and shared with other users. Recipients can use the connection without being able to view or alter the underlying settings.

## Changing Password

Go to **File → Change Password** to update the password for the current connection.

## Disconnecting

Go to **File → Disconnect** to close the active connection.
