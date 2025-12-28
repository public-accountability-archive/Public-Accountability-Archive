# Governance

## Purpose
The Public Accountability Archive (PAA) is governed under strict change-control rules to ensure factual integrity, auditability, and resistance to unauthorized or unilateral modification.

## Roles

### Repository Owner
- Maintains overall project direction
- Cannot directly modify protected branches
- Cannot self-approve pull requests

### Reviewer
- Holds write access
- Reviews and approves pull requests
- Cannot merge without satisfying branch protection rules
- Cannot modify repository rulesets

## Change Process
1. All changes are made in feature branches
2. All changes require a pull request
3. At least one independent review is required
4. Conversations must be resolved before merge
5. Force pushes and direct commits to `main` are blocked

## Integrity Controls
- Protected main branch
- Signed commits required
- Linear history enforced
- CI checks enforced when configured

These controls are intentional and non-negotiable.
They exist to preserve trust, not convenience.
