# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a Git tutorial repository used for learning Git workflows and branching strategies. The repository demonstrates feature branches, merge conflicts, and Git operations through a simple structure.

## Current State

The repository is currently in the middle of a cherry-pick operation with merge conflicts in README.md. The file contains conflict markers that need to be resolved.

## Git Workflow

This repository follows a feature branch workflow with the following branches:
- `master` - Main development branch
- `feature-A` - Feature branch for feature A development
- `feature-C` - Feature branch for feature C development  
- `Fix-B` - Bug fix branch
- `backup-master` - Backup of master branch

## Common Commands

Since this is a Git tutorial repository, the primary commands are Git-related:

```bash
# View current status
git status

# View branch list
git branch -a

# View commit history
git log --oneline

# Resolve merge conflicts (when in cherry-pick)
git add <resolved-file>
git cherry-pick --continue

# Or abort cherry-pick if needed
git cherry-pick --abort
```

## Repository Structure

The repository contains minimal files:
- `README.md` - Main documentation with feature lists (currently has merge conflicts)
- `.git/` - Git metadata and history

## Merge Conflict Resolution

When working with this repository, you may encounter merge conflicts in README.md. The file typically contains lists of features that may conflict when merging branches. Resolve conflicts by:

1. Editing the file to remove conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`)
2. Choosing which content to keep or combining both
3. Adding the resolved file with `git add`
4. Continuing the operation with appropriate Git command

## Development Notes

This repository serves as a learning tool for Git operations rather than a traditional software project. Focus on Git workflow understanding rather than code development when working here.