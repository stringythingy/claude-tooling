# claude-tooling Linear label taxonomy

Taxonomy version: `2026-06-09`

## Required label families

### `type/*` (required, exactly one)

- `type/bug`
- `type/feature`
- `type/chore`
- `type/docs`
- `type/research`

### `area/*` (required, at least one)

- `area/agents`
- `area/commands`
- `area/docs`
- `area/hooks`
- `area/ide-plugins`
- `area/install`

## Optional label families (propose-only)

These may be suggested in a repair comment but are not auto-added by the daemon:

- `source/customer`
- `source/team-request`
- `source/monitoring`
- `priority/p0`
- `priority/p1`
- `priority/p2`
- `status/blocked`
- `status/needs-info`

## Auto-add policy

The daemon may auto-add labels only from these families when evidence is unambiguous:

- `type/*`
- `area/*`

## Removal and replacement policy

Conservative mode is required for this repository:

- no automatic label removals
- no automatic label replacements
- when a removal/replacement seems needed, post a repair proposal comment instead

## Deprecated labels

Do not apply these labels:

- `type/improvement`
- `area/frontend`
- `area/backend`
- `source/internal`
