# Self-Hosted Listings

This document explains what a registry listing for a self-hosted AWC worker should point to and what the registry should leave to the contract itself.

## What A Listing Should Reference

A self-hosted listing should reference:

- the public contract defined with `awc-spec`
- compliance evidence generated with `awc-devkit/test-suite`
- the version of the tooling used to generate that evidence
- a repository URL or homepage for the worker

The listing may also include:

- `project.provider_id`
- `references.contract_ref`
- `listing.verification_status`
- `listing.listing_status`

## What The Registry Should Not Duplicate

The registry should not create a second definition for worker behavior such as:

- display title
- role summary
- capability tags
- restrictions
- escalation behavior

Those details should come from the contract and its attached evidence.

## Self-Hosted Integration Hints

If the contract includes optional self-hosted fields such as `metadata.platform_hints`, the registry can reference the contract that contains them. The registry should not copy those fields into a separate schema.

## Out Of Scope

- hosted runtime management
- user reviews
- ranking or recommendation logic
- proprietary trust scoring
