# Drone V4 — Research Progress

Report date: 24 November 2026
Research deadline: 14 December 2026

## Completed Milestones

| Milestone | Description | Verification |
|---|---|---|
| TM-41 | Second benchmark qualification | 83 tests passed |
| TM-42 | Recording-specific evidence intake | 111 tests passed |
| TM-43 | Evidence acceptance and deadline readiness | 137 tests passed |
| TM-44 | Final research evidence package | 166 tests passed |

## TM-45 Status

IN PROGRESS.

The research reporting milestone began,
but the development session stopped before
completion because of a usage limit.

The initial TM-44 verification gate and
29 focused tests passed.

The final TM-45 report has not yet been
completed or independently approved.

## Verified Indoor Research

Dataset: TUM RGB-D freiburg1_desk

| Model | Completed | Failed | Observed ATE RMSE |
|---|---:|---:|---|
| ORB-SLAM3 | 2 | 2 | 14.98-16.64 mm |
| RTAB-Map | 2 | 0 | 19.56-20.56 mm |
| OpenVINS | 0 | 0 recorded | Unmeasured |

Matched coverage:
573/573 eligible observations per completed run.

All 16 recorded accuracy metrics were
independently reproduced.

The comparison is limited to the tested
indoor sequence and documented protocol.

Runtime and memory comparisons are limited.

No overall model has been selected.

## Independent Reference Qualification

EuRoC V2_01_easy:
CONDITIONAL / BLOCKED.

ROVER:
NO-GO for independent outdoor scoring.

Bell412 Dataset 6:
NO-GO for independent outdoor scoring.

A complete GNSS outage remains unverified.

## Reproducibility

TM-44 saved-artifact verification: PASS.

This confirms artifact integrity,
report consistency and reproducible
documentation, not new experimental
validation or operational accuracy.

## Remaining Research Work

Complete TM-45 scientific reporting,
claim tracing and final review.

Deadline: 14 December 2026.
