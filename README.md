# AWC Registry

`awc-registry` defines the public submission and verification model for AWC workers.

Use this repository to understand:

- what a worker submitter needs to provide
- how verification is recorded
- how a listing moves from submission to public status

The registry references AWC contracts and evidence. It does not redefine the contract format; that remains in `awc-spec`.

## License

`awc-registry` is source-available under the Business Source License 1.1 (BUSL-1.1).

This repository is intended to support submission, verification, and listing lifecycle work for an AWC registry layer. Because it sits closer to marketplace, distribution, and commercial control concerns than `awc-spec` or `awc-devkit`, its license is intentionally more restrictive than those repositories.

See `LICENSE` and `docs/licensing.md` for the repository-specific terms and rationale.

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

- `docs/licensing.md`
- `docs/submit-a-worker.md`
- `docs/after-submission.md`
- `docs/submission-process.md`
- `docs/listing-lifecycle.md`
- `docs/certification-process.md`
