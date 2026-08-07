---
name: scan
description: Scan the entire codebase to build a dependency graph of the project. This is required before running any other commands that analyze the codebase.
---

# Scan the Codebase

This command scans the entire codebase and builds a dependency graph of the project. This graph is used by other commands to understand the relationships between different parts of the codebase.

`cxgrd scan `

This creates a `.cg` directory in the project root which contains the graph, symbol map and othe metadata. 
Thsi directory should not be commited to git, and should be added to `.gitignore` if it is not already.

## Prerequisites

Before running any cxgrd command, verify it's available:

`cxgrd --version`

If this fails (If cxgrd is not installed, tell the user and ASK BEFORE INSTALLING IT.), install it:

`npm install -g cxgrd`

Then retry the original command.