---
name: Update API docs on code changes
on:
  push:
    - repo: sunnybhara/nawa-ai-spark
      branch: main
context:
  - repo: sunnybhara/docs
automerge: false
---

Review the diff from the last merged PR in sunnybhara/nawa-ai-spark. Focus on changes to supabase/functions/ directory and any OpenAPI spec changes.

For each API change, update the corresponding documentation page. Include updated parameters, response examples, and code samples in curl, Python, and TypeScript.

Never use em dashes. Use "free" and "live" for key tiers. Product name is always "NAWA" in prose.

Success criteria: All API endpoint documentation matches the current codebase. A developer reading the docs can successfully call every endpoint.
