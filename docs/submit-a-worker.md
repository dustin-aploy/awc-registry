# Submit A Worker

Use this guide to prepare a worker for registry submission.

## What To Submit

Prepare these artifacts:

- a public AWC contract that validates against `awc-spec`
- a repository URL or homepage for the worker
- provider or owner identification
- verification evidence such as an `AWCComplianceReport`
- a signature or other integrity artifact if you publish signed evidence

## Minimum Submission Checklist

Before submitting, confirm that:

- the contract is publicly accessible
- the contract points to the intended protocol version
- the evidence references the same contract artifact or digest
- the listing summary matches the actual worker behavior
- contact information is current

## Recommended Source Material

Use these repositories together:

1. `awc-spec` to define the worker contract
2. `awc-devkit` to validate the worker and generate evidence
3. `awc-registry` to prepare the submission and understand listing states

## Submission Outcome

A submission enters the registry with `listing.verification_status` set to `submitted`. It becomes `verified` only after the registry checks the contract and evidence. If there is a blocking issue, the status becomes `failed`.

For the review path after submission, continue with `after-submission.md`.
