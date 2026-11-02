# Role release candidate validation — 1.19.14

All checks use disposable keys and synthetic projects; customer databases and licenses were not modified.

- 219 role-policy and backend assertions cover scopes, direct-edit denials, protected fields, self-approval, report submission, manager evidence, reinspection, free behavior and expired licenses.
- Eight owner-tool UI assertions cover roles, scope requirements, permission summaries and invalidation of stale generated keys after request/role/feature changes.
- UI checks cover role switching, nested context menus, Cut/Paste/transfer versus Copy, assessment actions without generic Edit mode, owned dialogs, denied-control re-enabling and protected Save As.
- Protected-project tests cover enrollment, unchanged readonly copies, signed saves and recovery, incremental exchange, tampering, stripped policies, reviewed imports, stale snapshots and Undo preserving enrollment.
- Seven cryptographic compatibility checks cover signed role/scopes, tampering, protocol downgrade rejection, old clients, legacy keys and unchanged ordinary-project fingerprints. App and Keygen public keys match, with no private RSA fields embedded in customer resources.
- Regression coverage includes current-tab/global search, replacement and tutorials, clipboard/delete/routing, lifecycle and assessment, evidence round trips, Item View, model library/brushes, offline content, themes, 20-language guides, export/Excel, incremental saving/sync, responsive snapshots and background saves.
- The Store build passes offline executable-content checks, including corrupt-module rejection. The MSIX contains the matching app, Theme Studio and four approved executable packs. Optional language/guide data remain downloadable.

Evidence logs are retained locally under .audit: roles11914.log, role-menu11914.log, role-approval11914.log, role-crypto11914.log, role-regressions11914.log, role-final11914.log, role-rest11914.log, role-exports11914.log and role-store11914.log, role-restore11914.log, role-final-store11914.log and role-online11914.log. Initial regression runs stopped on a Store-only test against the portable build and older UI test assumptions (scroll-suppressed tips, asynchronous history completion and preferring the verified paired Theme Studio); corrected reruns passed. This is validation of the listed paths, not a claim of a penetration audit or all possible driver/account combinations.

The local Store candidate manifest and immutable fingerprint are recorded in .audit/Store-1.19.14/candidate.json. No Store upload or submission was performed. Owner acceptance testing remains required.
