# koi-ashell-builder

Minimal public builder for an unsigned **a-Shell noPython** IPA from the official source:

<https://github.com/holzschu/a-shell>

The recovery workflow is manually triggered, uses the official `a-Shell-noPython` target on a standard GitHub-hosted macOS runner, disables code signing, packages the app as an unsigned IPA, and uploads `a-Shell-noPython-official-unsigned`.

This repository contains no KOI source, database, music, personal information, credentials, or secrets.

## Recovery status

`IPA_RECOVERY=PASS`

- Build: [GitHub Actions run 39354750364](https://github.com/koinsy/koi-ashell-builder/actions/runs/39354750364)
- Artifact: `a-Shell-noPython-official-unsigned`
- Device verification: app launched successfully and executed `echo KOI_READY`
- Retained: terminal, shell commands, JavaScript, local files, and network-capable command support
- Excluded: Python, pico, and multimarkdown
- Installation: the unsigned IPA must be signed and sideloaded; free Apple ID signing requires periodic refresh
