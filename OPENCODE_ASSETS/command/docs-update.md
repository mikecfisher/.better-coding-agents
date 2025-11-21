---
description: Update the linked codebases to the latest version
agent: build
---

# Update Command

This command updates all the linked codebases (effect, opencode, tanstack-db, and powersync-js) to their latest versions by pulling fresh changes from the upstream repositories.

You will need to run the following commands in this directory: `~/.better-coding-agents`

## Instructions

Execute the following git subtree pull commands in sequence to update each repository:

1. **Update Effect repository**

   ```bash
   git subtree pull --prefix resources/effect https://github.com/Effect-TS/effect.git main
   ```

2. **Update OpenCode repository**

   ```bash
   git subtree pull --prefix resources/opencode https://github.com/sst/opencode.git main
   ```

3. **Update TanStack DB repository**
   ```bash
   git subtree pull --prefix resources/tanstack-db https://github.com/TanStack/tanstack-db.git main
   ```

4. **Update PowerSync JS repository**
   ```bash
   git subtree pull --prefix resources/powersync-js https://github.com/powersync-ja/powersync-js.git main
   ```

Each command will fetch the latest changes from the upstream repository and merge them into the local subtree. There should be no conflicts, if there are ask the user what they want to do.
