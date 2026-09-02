# Development log

## 2026-09-02 — canonical multi-track disc identity

The public `v0.3.3` manifest used the merged whole-disc BIN identity, while
the verifier hashes the first BIN named by the CUE. Release `v0.3.4` uses the
canonical Track 01 identity and keeps the merged identity as a compatibility
entry. Verification passed with the owned two-track Europe disc and rejected
an unrelated disc.

## 2026-09-01 — setup executable-name parity

The public `v0.3.0` source used different CMake and setup-relaunch executable
names. The corrected source uses `Mega_Man_Legends_Recompiled` in all three title-owned paths.
`Test-SetupExecutableNameParity.ps1` passes. Exact-ZIP automatic relaunch is
still required before release.
