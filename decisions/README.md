# Decision records

A decision record states 1 decision of the project and the reason for it.
The project numbers the records from 0001 on and keeps them in this folder.
The file name of a record starts with its number and its title.
The folder then lists the records in order.
To change a decision, a PR edits its record (see 0030).
To drop a decision, a PR deletes its record.
The project doesn't use the number of a deleted record again.
Git keeps the earlier versions.

## Format

Each record has these parts:

- A title line with the number and the title.
- A line with the date of the decision.
- Decision: what the project does.
- Reason: why the project does it.
- Consequences: what follows from the decision, with the costs.
- Changes: 1 line for each change of the decision, with the date, the PR and the reason.
  A record gets this part with its first change.
