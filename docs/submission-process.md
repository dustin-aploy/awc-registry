# Submission Process

## Purpose

`awc-registry` provides a small public submission flow for AI Work Contract (AWC) workers and related projects. The registry accepts evidence-backed submissions for self-hosted workers and keeps the submission surface intentionally small.

## What A Developer Submits

A developer or provider should submit:

- a public contract artifact that validates against `awc-spec`;
- a repository or homepage for the worker or project;
- a compliance report or similar verification evidence;
- a signature or equivalent public integrity artifact when available; and
- basic registry metadata such as provider identity and listing summary.

## Minimal Registry Fields

The current registry entry schema keeps the submission surface small:

- `project.provider_id` identifies the submitting provider in a stable registry-friendly way;
- `references.contract_ref` points to the public contract artifact;
- `submission` records when and by whom the entry was submitted;
- `listing.verification_status` records the current verification result; and
- `listing.listing_status` records whether the verified entry is publicly listed.

## V1 Verification Flow

The Phase 1 flow is intentionally simple:

1. The developer submits a registry entry with a contract reference and public evidence.
2. The registry checks that the contract and evidence are loadable and coherent.
3. The registry records a verification result.
4. Verified entries may then be marked as listed.

This repository does not implement hosted execution, ranking, or review aggregation as part of that flow.
