# Auto Execution

The **Auto Execution** feature allows LextEdit to automatically run a command multiple times at a defined interval, stopping when a specified condition is met. This is useful for polling a system during long-running operations without manually re-executing a query.

## Accessing Auto Execution

Go to **File &rarr; Auto-Execute** to open the Auto Execution configuration.

## How It Works

Auto Execution is useful for:

- Polling a system until a specific result appears. For example, waiting for a background process to set a status flag to a completed value before proceeding with the next step.
- Running repeated checks during testing or development. For example, monitoring a row count or a queue depth as you work through a test scenario.
- Automating multi-step processes where each step depends on the previous result. Auto Execution can reduce the need to manually re-run a query every few seconds.

Configure the command to execute, the repeat interval, and the stop condition. LextEdit will continue executing the command at the specified interval until the stop condition is satisfied. Results from each execution are displayed in the grid and updated on each pass.

## Stop Conditions

The stop condition is evaluated after each execution. When the condition is met, Auto Execution halts automatically. If the condition is never met, the execution continues indefinitely until you cancel it manually using **File &rarr; Cancel**.

## Use with Transaction Control

When using Auto Execution with commands that modify data, consider whether AutoCommit should be enabled or disabled. If AutoCommit is off, changes accumulate in an open transaction across executions. Use **Tools &rarr; Commit** or **Tools &rarr; Rollback** to finalize the transaction once Auto Execution stops.
