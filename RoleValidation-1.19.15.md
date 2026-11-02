# Role presentation validation — 1.19.15

Role UI checks verify Full Control, multiple department scopes, live changes to View Only, explicit legacy-license wording and the free-edition label. The shared presentation is used by About and License activation. The existing 219 backend permission assertions, protected-project cases and Store offline module checks also pass. The 20 UI catalogs include the four new phrases, and the translated role guide explains where to find the role. Built-in fallback labels support older cached language packs.

Evidence: .audit/about-role11915.log and .audit/about-final11915.log. The MSIX manifest/payload matches the local candidate; .audit/Store-1.19.15/candidate.json records its checksum. No customer licenses or projects were changed. Microsoft Store submission remains on hold.
