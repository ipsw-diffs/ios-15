# iOS 15 legacy migration closure

Recorded: 2026-08-13

## Claim and scope

Question: can the complete iOS 15 payload set present at legacy commit
`d881e84676308404c6947d0218c11f347a6f3a89` be copied exactly into this
archive shard and later cataloged with immutable source and destination pins?

- First lifecycle stage: select every top-level legacy payload whose README
  identifies iOS major version 15 and whose build train is iOS 15 (`19*`).
- Last lifecycle stage: a catalog entry independently verifies the source tree
  against this shard's merged default-branch commit.
- Supported claim after closure: the selected Git subtree was faithfully
  migrated and cataloged with immutable provenance.
- Excluded: regenerating the diff from IPSWs, identifying the exact historical
  `ipsw` generator version, and assigning semantics beyond the copied report.

## Authority map

| Property | Authority |
| --- | --- |
| Migration membership | Complete matching top-level tree at the pinned legacy commit |
| Versions, builds, and IPSW inputs | Strictly parsed source README |
| Files, bytes, modes, and tree identity | Git objects at the pinned legacy commit |
| Destination payload and manifest | Validated migration specification and mechanical staging |
| Catalog destination pin | Merged shard default-branch commit |

## Closure matrix

| Stage | Evidence | Status before publication |
| --- | --- | --- |
| Selection and trigger | One matching root: `15_8_6_19H402__vs_15_8_7_19H411` | Closed |
| Inputs and resources | README contains exactly two matching `iPodtouch_7` IPSW inputs | Closed |
| Transformation | Mechanical staging and independent revalidation reproduce tree `721ca55fb96c8b41ba4de83693c2ab40ff229056` | Closed |
| Advertisement and options | Generated shard README lists exactly one comparison | Closed |
| Dispatch and transport | One unsigned shard commit and pull request | Unresolved |
| State transition | Shard merge precedes catalog publication | Unresolved |
| Outcome oracle | Catalog audit matches source and merged destination | Unresolved |

## Expected inventory

The selected payload contains exactly 1 tracked file and 10,605 logical bytes.
Its source subtree is
`721ca55fb96c8b41ba4de83693c2ab40ff229056`; the staged payload has the same
tree identity. The migration additionally generates one provenance manifest.

## Negative-evidence audit and stop conditions

The absence of other matching roots is scoped only to the pinned legacy tree;
it does not claim that no iOS 15 diff ever existed outside the repository or in
unreachable history. A README-only payload is still a valid Git subtree, but it
does not prove the firmware had no unreported semantic changes. Stop if the
source commit, selected path, README metadata, inventory, tree identity,
destination merge commit, or catalog audit differs.

## Review-time bounded conclusion

Selection, input validation, exact staging, and archive advertisement are
closed. Publication, the merged destination state, and catalog verification
remain unresolved until their corresponding GitHub transitions occur.
