# What Happens After Submission

After a worker is submitted, the registry follows a short review and listing flow.

## Step 1: Intake

The registry confirms that the submission is complete enough to review. At this point the verification status is `submitted`.

## Step 2: Verification

The registry checks:

- the contract can be loaded
- the contract aligns with a released AWC protocol version
- the evidence is readable and matches the claimed worker
- the listing metadata is coherent with the submitted artifacts

If the review succeeds, the verification status becomes `verified`. If there is a blocking issue, it becomes `failed`.

## Step 3: Listing Decision

Verified entries can then be marked:

- `unlisted` if they are verified but not publicly shown yet
- `listed` if they are publicly shown
- `paused` if they need to be hidden temporarily
- `retired` if they are no longer active

## Step 4: Ongoing Maintenance

A listing may need a new submission or recertification when:

- the contract changes materially
- the evidence is no longer current
- the protocol version changes
- the listing is downgraded, paused, or retired

For stronger review requirements, see `certification-process.md`.
