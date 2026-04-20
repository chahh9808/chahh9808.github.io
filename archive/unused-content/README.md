# Unused Content Archive

This folder stores content that was previously present in `content/` but is currently not used on the live site.

## Why this exists
- Keep active content folders clean and less confusing
- Preserve old files without deleting history
- Make restore easy if any page is needed again

## Archived on 2026-04-18
- `content/projects.md`
- `content/experience.md`
- `content/event/example/index.md`
- `content/teaching/_index.md`
- `content/teaching/js/index.md`
- `content/teaching/python/index.md`
- `content/project/pandas/index.md`
- `content/project/pytorch/index.md`
- `content/project/scikit/index.md`

## Restore guide
1. Move the file back to its original path under `content/`
2. Remove `_build.render: never` and `_build.list: never` if present
3. Reconnect it from homepage/menu if needed
4. Check with local preview before merge
