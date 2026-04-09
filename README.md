# bonfyre-tel

Telephony entry repo for Bonfyre.

This repo is a public entry vector for the telephony surface:

- FreeSWITCH Event Socket listener
- SIP/SMS/MMS call flows
- mock server for zero-cost testing
- SQLite-backed call and message logging
- verification code workflows

## Why This Exists

The live `BonfyreTel` runtime currently lives in:

- `/Users/nickgonzales/Projects/bonfyre-oss/cmd/BonfyreTel`

This repo gives that surface its own clear entry point so the Bonfyre page can link to it directly.

## Current Layout

- `cmd/bonfyre-tel/`
  - extracted telephony binary source and deploy examples
- `docs/`
  - extraction notes

## Dependency Note

`bonfyre-tel` is lighter than the other new entry repos.

It currently builds with:

- system sockets/network headers
- `sqlite3`

It does not currently need a vendored `bonfyre-core` slice for local extraction validation.
