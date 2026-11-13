# Sealed consumer materialization

This revision supersedes the independently materialized databases in
`da970031985b25868d93d8322488824eaa351b71`. Only the reviewed package’s exact
consumer projection and exact public ZIP candidates are used; no SQLite import,
regeneration, ZIP rewrap or mixture with the earlier candidates is performed.
The internal academic graph remains `researcher-demo`.

## Chain of custody

- Input: `graph-pipeline-package-0da33f6.tar.gz`, 34,208,475 bytes.
- Full archive SHA-256:
  `0daca1876c3b3c55d1de5ab955c27ad08858ffec83a4da3ea49768fe6d20f7e2`.
- Sealed `graph-snapshot.json` SHA-256:
  `9f6308da6feddc40325efc5f437ba51b31a88aa99e6b8d6a7384ced669b84bd5`.
- Generator source/tool root: `47aa890ecfba566c2608d14ee4daeee7bdf8901e`.
- Original library: `f113828a712e874c4318ee569bc4e47336ab80e5`.
- Projection/package implementation: private packaging repository
  `0da33f66dc12577102e8fff325938b2c371e7eb6`, independently approved at
  `b3aceecda87fa50733375604e84c8b1bf0417c67` with matching implementation bytes
  (approval supplied by the orchestrator, not inferred from a remote branch).
- Released through 2026-11-11; schema 65.40; baseline 2026-09-30;
  42 subsequent released days. Future pending days are not imported.
- Released-recipe digest:
  `df0f93fa69ddc11b3ccd59a9bfc952222c0e2c717506c19b5b2e14e618ef9905`.

The package seal covers all 28 internal files. Its projection checksum list,
`SNAPSHOT.md` and `graphs-manifest.json` are retained except that private
repository names are replaced with neutral labels. Otherwise the manifest’s
commit pins and source/export/tool/runtime fields remain frozen; it is not
rewritten to pretend that the generator source commit is the consumer commit.
Its upstream ZIP hashes refer to the original generator wrappers; public ZIP names/hashes are in each
graph’s `zip`/`zipSha256` fields. Only those exact public ZIPs are staged for review.

A future release target plan must record the final **consumer commit** separately
from the source root. The portable incremental review bundle and target plan live
outside this Git tree. No release is created by this update. Search indexes and
recorder baselines are derived/private package inputs and are not consumer files.

## Preservation and scope

Original source material, artwork inputs, notices and the older developer trial
remain recoverable at consumer base `a30cc950a57f19780dc7a24979c08df2db68435c`
and the pinned original library. No history or refs are rewritten or deleted.
The four public roots contain only regular `db.sqlite` files and referenced
assets; all original graph images/addresses/content/UUIDs remain intact.
Existing asset notices, attribution and undecided licensing remain unchanged.

Validation opens temporary copies only: sealed-package/raw-folder/public-ZIP
byte equality, SQLite integrity and logical/runtime state, source recipe digests,
baseline identities, local asset references and bytes, reproducible ZIP checksums,
and incremental privacy/secret scans. Independent source-semantics approval is
reused, not represented as a fresh content generation. No desktop visual,
recording, draft-release or Studio acceptance is claimed; that proof is running
separately. Production source, workflows, visibility, access and settings stay
unchanged. Independent re-review is required before merge/publication/cutover.
