# pickle_clubs v1.1.3

## Fixes

- Enforce staff permissions, drink recipes, service proximity and timing on the server.
- Bill drink orders on delivery and check inventory and society transactions.
- Improve employee, admission, VIP, escort and disconnect handling.
- Fix management input updates and ship the rebuilt NUI bundle.

## Upgrade notes

- Verify the installed inventory and society account adapters.
- The existing VCR_OSD_MONO.ttf reference may fall back to another font if that optional font is unavailable.

## Package and validation

- The ZIP contains one pickle_clubs/ folder with the complete resource, installation files, license and runtime NUI assets where applicable. Unbuilt web/ sources, node_modules/ and Git metadata are excluded.
- Required local NUI scripts and stylesheets were checked before packaging. Prior remediation validation passed targeted mocked regressions and Lua/JavaScript syntax checks; this is not a live FiveM integration test.
- Test the resource with your installed frameworks, inventory, database and other integrations before use. Transactions spanning framework persistence, SQL and local KVP still have crash-recovery boundaries.

Source: [audit remediation PR #3](https://github.com/PickleModsCommunity/pickle_clubs/pull/3), branch `fix/audit-remediation`. This release includes the PR changes without merging the PR.
