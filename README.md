# Commit Automation in `vaillantm/auto`

The `vaillantm/auto` repository automates commit generation based on a configurable weekly schedule. This process focuses on daily commit quotas that dictate how many commits can occur each day.

## Daily Commit Quotas

Each day has a predefined limit on the number of commits:

- **Monday**: 3 commits
- **Tuesday**: 2 commits
- **Wednesday**: 1 commit
- **Thursday**: 4 commits
- **Friday**: 5 commits
- **Saturday**: 0 commits
- **Sunday**: 2 commits

## Process Overview

1. **Weekly Schedule**: Supports varying commit frequencies for each day.
2. **Commit Logic**: Scripts check the current day and create commits if the daily quota hasn't been reached, using messages from a word list.
3. **State Tracking**: A state file (e.g., `.week_state`) tracks weekly commits to ensure quotas are respected.
4. **Automation**: GitHub Actions workflows execute the commit process automatically at scheduled intervals.

This setup maintains a consistent commit history while adhering to specified limits for each day of the week.
