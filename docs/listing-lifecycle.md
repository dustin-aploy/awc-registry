# Listing Lifecycle

## Goal

The registry tracks a small set of statuses for submission, verification, and public listing. This keeps the V1 registry useful without turning it into a full end-user marketplace.

## Verification Status

`listing.verification_status` captures the verification outcome:

- `submitted`: the registry received the entry but has not completed verification yet;
- `verified`: the registry confirmed the contract reference and evidence are coherent enough to publish;
- `failed`: the registry found a blocking issue in the submitted contract, evidence, or metadata.

## Listing Status

`listing.listing_status` captures whether a verified entry is publicly shown:

- `unlisted`: the entry exists in the registry but is not publicly listed yet;
- `listed`: the entry is publicly listed;
- `paused`: the entry was listed before but is temporarily hidden or flagged;
- `retired`: the entry is no longer active and should stay out of new listings.

## Out Of Scope

This lifecycle does not encode:

- user review counts or sentiment;
- ranking or recommendation logic;
- proprietary trust scores; or
- application-specific matching and pricing behavior.
