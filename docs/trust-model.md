# Trust Model

The registry helps consumers answer one question: what public evidence supports this worker's AWC claim?

It does not create trust on its own. It records trust signals that can be inspected:

- the contract defined in `awc-spec`
- the evidence generated with `awc-devkit/test-suite`
- the review and listing decisions recorded by the registry

## Who The Registry Relies On

- protocol maintainers define the contract format and protocol versions
- test-suite maintainers define how compliance evidence is produced
- project publishers provide contracts, reports, signatures, and project metadata
- registry reviewers check that submissions are coherent and correctly represented
- consumers decide how much weight to assign a listing

## Trust Boundaries

The registry does not claim that:

- a listed project is safe in every deployment
- a listed project is secure in every environment
- a certified project will remain compliant forever
- the registry is the source of truth for contract semantics

The registry only claims that the listing contains evidence that can be checked against public rules.

## What Makes A Listing More Credible

Credibility increases when:

1. the listing references a released AWC protocol version
2. the evidence comes from public AWC tooling rather than an ad hoc format
3. the report is public and signed when signatures are used
4. the reviewer verified version alignment and evidence integrity
5. the listing is still within its review or recertification window

This is why the registry distinguishes different verification levels instead of treating all listings as equivalent.
