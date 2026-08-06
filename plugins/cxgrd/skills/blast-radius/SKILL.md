---
name: blast-radius
description: Analyze the blast radius of a code change before making it. Use before generating a diff that touches more than one file, before refactoring shared code, or when the user's request could affect files beyond the ones being directly edited.
---

# Blast Radius Analysis

Before making a change that could affect other files, run:

`cxgrd input "<description of the change>" --json`

This returns a JSON object with affected files, risk level, and recommendations. Read the output and factor high-risk affected files into your plan before editing.

## Pre-requisites
This command requires that the project has been scanned with `cxgrd scan`.
If the project hasn't been scanned yet (`cxgrd input` returns a NO_GRAPH error), run `cxgrd scan` first, then retry.
