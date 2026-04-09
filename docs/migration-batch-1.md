# Migration Batch 1

This is the first extraction batch for `bonfyre-tel`.

## Goal

Move the live `BonfyreTel` binary into its own public-facing repo so the telephony surface can be linked and understood independently.

## Batch Contents

### 1. `BonfyreTel`

Current source:

- `/Users/nickgonzales/Projects/bonfyre-oss/cmd/BonfyreTel`

Target:

- `cmd/bonfyre-tel/`

## Acceptance Criteria

1. `bonfyre-tel` builds from the extracted path
2. the deploy examples and README move with it
3. the repo can serve as a clean backlink target from the live Bonfyre page

## Progress

- imported:
  - `BonfyreTel`
- verification:
  - `bonfyre-tel` builds from the extracted path
  - usage surface runs from the extracted binary
