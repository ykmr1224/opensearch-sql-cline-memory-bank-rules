# Memory Bank System

Memory resets between sessions. Memory Bank provides complete project context and must be read at start of every session.

## Core Files (Required)
1. `projectbrief.md` - Foundation, requirements, scope
2. `productContext.md` - Purpose, problems solved, user goals
3. `activeContext.md` - Current work, recent changes, next steps
4. `systemPatterns.md` - Architecture, design patterns, relationships
5. `techContext.md` - Technologies, setup, dependencies
6. `progress.md` - Status, completed work, known issues

## Feature Investigation
- `memory-bank/features/feature-[name].md` - New feature investigations
- `memory-bank/features/enhancement-[name].md` - Feature enhancements
- `memory-bank/features/investigation-[topic].md` - Technical investigations

## Workflows

### Plan Mode
1. Read Memory Bank → 2. Check completeness → 3. Develop strategy → 4. Present approach

### Act Mode
1. Read Memory Bank → 2. Update documentation → 3. Execute task → 4. Document changes

## Session Start Protocol
**CRITICAL**: Always start by reading ALL memory bank files to understand project state, then:
1. Summarize key findings and current context
2. Identify next steps from activeContext.md and progress.md
3. Read relevant feature files when mentioned or referenced
4. Proceed with task using this context

## Updates
Update Memory Bank when:
- Discovering new project patterns
- After significant changes
- User requests "update memory bank"
- Context needs clarification
