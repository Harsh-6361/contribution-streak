# Contribution Streak Plan

## Goal
Increase GitHub daily contributions for streak.

## Current Status
- Repo: https://github.com/Harsh-6361/contribution-streak
- Auth: gh account Harsh-6361

## Automated Tasks

### Daily Actions (run these commands)
```bash
cd /path/to/contribution-streak
echo "commit $(date +%Y%m%d-%H%M%S)" >> streak.md
git add .
git commit -m "streak $(date +%Y-%m-%d)"
git push
```

### To do 100+ commits at once:
```bash
cd /path/to/contribution-streak
for i in {1..100}; do echo "day $i" >> streak.md && git add streak.md && git commit -m "day $i"; done
git push
```

## Notes
- Each push with new commit counts as contribution
- For streak: need commits on separate days
- Contributions reset at midnight UTC
