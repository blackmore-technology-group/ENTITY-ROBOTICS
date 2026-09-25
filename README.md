# ENTITY-ROBOTICS

**ENTITY v3.4.0 executable Robotics implementation package.**

This repository configures the **one ENTITY Global Passport** for robotics and autonomous-system workflows. It does not define a separate passport protocol and does not modify ENTITY core semantics.

[ENTITY](https://github.com/blackmore-technology-group/ENTITY) · [v3.4.0 release](https://github.com/blackmore-technology-group/ENTITY/releases/tag/v3.4.0) · [Global Passport documentation](https://github.com/blackmore-technology-group/ENTITY/blob/main/docs/v3.4/GLOBAL_PASSPORT.md) · [Domain packages](https://github.com/blackmore-technology-group/ENTITY/blob/main/docs/v3.4/DOMAIN_PACKAGES.md)

## What this package is for

Use ENTITY-ROBOTICS as the starting point when you need persistent provenance, scoped authority, rights and evidence around robots, autonomous systems, tasks, operating context or derived outputs while keeping device possession, hosting and infrastructure control separate from sovereign authority.

The v3.4 package includes mappings for **ROS 2** and **Open-RMF**. Those mappings describe correspondence; ENTITY does not redefine the external standards.

Typical evaluation paths include:

- preserving provenance across robot, fleet, task or software-state changes;
- binding scoped authority and evidence to machine actions or generated outputs;
- carrying rights and governance context across providers or orchestration systems;
- composing jurisdiction, safety, trust and technical profiles inside one Global Passport.

## Deploy the package

Required deployment facts:

- `organization`
- `jurisdiction`
- `authority_source`
- `safety_policy`

`deployment.example.json` is intentionally non-production until every `CONFIGURE-ME` value is replaced with organization-specific facts.

```text
Select package → configure organization facts → connect systems/data → ingest → verify passport → run conformance → deploy
```

## Verify locally

```bash
python tools/verify_package.py
```

The verifier checks the repository inventory and the package/source-release binding.

## Release binding

- Core source: `blackmore-technology-group/ENTITY` PR #41
- Source head: `2d7529fbadb4dd04840d62b751294bf9a7f70ed5`
- Release snapshot: `3ff0e51ca2daabf50bc517e9c6e3438e8c150f1560cca6c99621621e3c855a90`
- Package SHA-256: `3a0e68fa6c63b2ef9cf79ccf463335af72d49ffb3cd028c88b6a998d8678f38f`

## Go deeper

- [ENTITY v3.4.0](https://github.com/blackmore-technology-group/ENTITY/releases/tag/v3.4.0)
- [Developer portal](https://github.com/blackmore-technology-group/ENTITY/blob/main/DEVELOPERS.md)
- [Engineering evidence](https://github.com/blackmore-technology-group/ENTITY/blob/main/docs/ENGINEERING_EVIDENCE.md)
- [Open contributor tasks](https://github.com/blackmore-technology-group/ENTITY/issues?q=is%3Aissue+is%3Aopen)

## Truth and compliance boundary

External standards remain externally authoritative and are mapped, not redefined. Package verification does **not** establish regulatory compliance, objective external truth, system safety, legal title or accounting fair value. Provider custody does not create ENTITY authority.

Deployment-specific safety, legal, security, certification and operational determinations remain the responsibility of the deploying organization.
