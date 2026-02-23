# Command-Line Arguments

LextEdit supports command-line arguments that can be added to a Windows shortcut to pre-configure connection settings, window position, or file loading.

## Arguments

| Argument | Description |
|---|---|
| `-f` | Open a LextEdit window and load a specific file |
| `-t` | Connection type: `MSQL` for a MOCA server, or `ODBC` for a SQL database |
| `-a` | IP address or DNS name of the system to connect to |
| `-p` | Port number the system is accessible on |
| `-d` | ODBC driver to use for a file or system connection |
| `-c` | Catalog or database name (used with SQL/ODBC connections) |
| `-u` | Username for the connection login |
| `-w` | Password for the connection login |
| `-l` | Window position and size: `left,top,width,height` in pixels |

## Examples

**Example 1 — Open the Connection window pre-set to MOCA:**

```
LextEdit.exe -t MSQL
```

Automatically opens the Connection Information dialog on the Moca Servers tab when LextEdit starts.

**Example 2 — Set window position and size:**

```
LextEdit.exe -l 0,75,880,920
```

Creates the window at 0 pixels from the left, 75 pixels from the top, 880 pixels wide, and 920 pixels tall.

**Example 3 — Auto-login to a MOCA connection:**

```
LextEdit.exe -a 192.168.1.101 -p 811 -t MSQL -u SUPERVISOR -w SUPERVISOR01
```

Connects automatically to the MOCA system at `192.168.1.101` on port `811` using the SUPERVISOR credentials.

## Setting Up a Shortcut

1. Locate the LextEdit executable (typically in `C:\Program Files\LextEdit\`).
2. Right-click → **Create shortcut**.
3. Right-click the shortcut → **Properties**.
4. In the **Target** field, append your desired arguments after the executable path.
5. Click **OK**.
