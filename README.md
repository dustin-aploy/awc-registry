# AWC Registry

`awc-registry` defines the public submission and verification model for AWC workers.

Use this repository to understand:

- what a worker submitter needs to provide
- how verification is recorded
- how a listing moves from submission to public status

The registry references AWC contracts and evidence. It does not redefine the contract format; that remains in `awc-spec`.

## Submission Model

A submission typically includes:

- a public AWC contract
- project or provider metadata
- verification evidence such as a compliance report
- integrity material such as a signature when available

## Verification Model

The registry records whether the submission is:

- `submitted`
- `verified`
- `failed`

Verification checks whether the referenced contract and evidence are loadable, coherent, and consistent with the claimed listing level.

## Listing Lifecycle

After verification, a listing can move through these states:

- `unlisted`
- `listed`
- `paused`
- `retired`

## Developer Docs

- `docs/submit-a-worker.md`
- `docs/after-submission.md`
- `docs/submission-process.md`
- `docs/listing-lifecycle.md`
- `docs/certification-process.md`
