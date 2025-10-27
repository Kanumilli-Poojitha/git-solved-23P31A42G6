cat > GIT_JOURNEY.md <<'EOF'
# My Git Mastery Challenge Journey

## Student Information
- Name: Kanumilli-Poojitha
- Student ID: 23P31A42G6
- Repository: https://github.com/Kanumilli-Poojitha/git-solved-23P31A42G6
- Date Started: 2025-10-26
- Date Completed: 2025-10-27

## Task Summary
Cloned instructor's repository with pre-built conflicts and resolved all merge conflicts across multiple branches using proper Git workflows.

## Commands Used

| Command | Times Used | Purpose |
|---------|------------|---------|
| git clone | 1 | Clone instructor's repository |
| git checkout | 20+ | Switch between branches |
| git branch | 10+ | View and manage branches |
| git merge | 2 | Merge dev and conflict-simulator into main |
| git add | 30+ | Stage resolved conflicts |
| git commit | 15+ | Commit resolved changes |
| git push | 10+ | Push to my repository |
| git fetch | 2 | Fetch updates from instructor |
| git pull | 1 | Pull updates |
| git stash | 2 | Save temporary work |
| git cherry-pick | 1 | Copy specific commit |
| git rebase | 1 | Rebase feature branch |
| git reset | 3 | Undo commits (soft/mixed/hard) |
| git revert | 1 | Safe undo |
| git tag | 2 | Create release tags |
| git status | 50+ | Check repository state |
| git log | 30+ | View history |
| git diff | 20+ | Compare changes |

## Conflicts Resolved

### Merge 1: main + dev (6 files)

#### Conflict 1: config/app-config.yaml
- *Issue*: Production used port 8080, development used 3000
- *Resolution*: Created unified config with environment-based settings
- *Strategy*: Keep production as default, add dev as optional
- *Difficulty*: Medium
- *Time*: 15 minutes

#### Conflict 2: config/database-config.json
- *Issue*: Different database hosts and SSL modes
- *Resolution*: Created separate profiles for production and development
- *Strategy*: Restructured JSON to support both environments
- *Difficulty*: Medium
- *Time*: 10 minutes

#### Conflict 3: scripts/deploy.sh
- *Issue*: Different deployment strategies (production vs docker-compose)
- *Resolution*: Added conditional logic based on DEPLOY_ENV variable
- *Strategy*: Made script handle both environments dynamically
- *Difficulty*: Hard
- *Time*: 20 minutes

#### Conflict 4: scripts/monitor.js
- *Issue*: Different monitoring intervals and log formats
- *Resolution*: Environment-based configuration object
- *Strategy*: Used process.env.NODE_ENV to determine behavior
- *Difficulty*: Medium
- *Time*: 15 minutes

#### Conflict 5: docs/architecture.md
- *Issue*: Different architectural descriptions
- *Resolution*: Merged both descriptions into comprehensive document
- *Strategy*: Created sections for each environment
- *Difficulty*: Easy
- *Time*: 10 minutes

#### Conflict 6: README.md
- *Issue*: Different feature lists and version numbers
- *Resolution*: Combined all features with clear environment labels
- *Strategy*: Organized features by category
- *Difficulty*: Easy
- *Time*: 10 minutes

### Merge 2: main + conflict-simulator (6 files)
- Conflicts resolved similarly: kept production defaults, moved experimental/dev items behind flags, documented merges in commit messages.

## Most Challenging Parts
1. Understanding conflict markers (<<<<<<<, =======, >>>>>>>) and which side was HEAD.
2. Choosing the correct content to keep (production vs development).
3. Resolving complex logic (scripts/deploy.sh) without introducing regressions.
4. Recovering lost commits via git reflog after resets.

## Key Learnings
- Mastered conflict resolution and the meaning of conflict markers.
- Practiced advanced git operations (rebase, cherry-pick, reset, reflog).
- Learned to stage and commit carefully and to document changes.

## Reflection
This challenge taught me that merge conflicts are normal; with careful reading and testing you can resolve them safely. Using git reflog and cherry-pick helped me recover from mistakes.

EOF