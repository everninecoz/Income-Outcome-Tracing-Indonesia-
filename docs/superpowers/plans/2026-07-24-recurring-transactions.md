# Recurring Transactions Implementation Plan

**Goal:** Add user-confirmed monthly recurring transaction reminders to IOT.

**Constraints:** Runtime remains only in `iot.html`; existing transaction and backup data stay compatible; recurring data uses the new `recurring_rules` Supabase key.

### Task 1: State and persistence

- [ ] Add `recurringRules`, `RECURRING_KEY`, load/save helpers, and input validation.
- [ ] Verify malformed/missing stored rules fall back to an empty list.

### Task 2: Reminder and recording flow

- [ ] Add a due-rule panel that only shows rules whose `nextDue` is today or earlier.
- [ ] Add explicit “Catat” behavior that uses the existing `finalizeEntry` flow and advances `nextDue` one month after a successful save.

### Task 3: Rule management and release

- [ ] Add a Menu modal to create and remove monthly rules.
- [ ] Add static checks, bump version to v1.12, update README, commit, and push.
