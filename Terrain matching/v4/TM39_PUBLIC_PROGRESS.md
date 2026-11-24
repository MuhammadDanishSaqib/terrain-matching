# TM-39 offline benchmark evaluation progress

Completed locally on 24 November 2026. Research deadline 14 December 2026.

## Software

A standalone offline command-line tool evaluates saved position trajectories against independently measured references. It checks reviewed clock and frame evidence, reference independence, reference uncertainty, and input checksums before scoring. Its JSON report includes position-error statistics, matched coverage, rejected observations, and gaps. Incomplete evidence produces an unqualified report with no accuracy score.

## Verification

| Check | Result |
| --- | --- |
| New automated evaluator tests | 28 passed, 0 failed |
| Existing relevant regression tests | 24 passed, 0 failed |
| Saved indoor metric reproduction | All four completed runs and 16 stored metrics reproduced exactly |
| Outdoor qualification checks | Two expected rejections with no accuracy score |

## Indoor benchmark results

All four completed runs used the same TUM RGB-D `freiburg1_desk` sequence and matched 573 of 573 eligible input observations. Reproduction preserved the original rigid alignment and did not rerun the model binaries.

| Model | Completed runs | Failed attempts in the original benchmark | Best ATE RMSE |
| --- | ---: | ---: | ---: |
| ORB-SLAM3 RGB-D | 2 | 2 | 14.98 mm |
| RTAB-Map RGB-D | 2 | 0 | 19.56 mm |

OpenVINS has no comparable completed result. The measurements describe one indoor sequence. Outdoor accuracy and overall model selection remain unresolved.

## Outdoor qualification and deadline

ROVER Garden Small requires recording-specific survey timing, frame and calibration evidence. Bell412 Dataset 6 requires independently characterized reference positions, uncertainty and timing evidence. Both remain unqualified for independent outdoor scoring.

The offline evaluator and reproduced indoor measurements are ready ahead of 14 December 2026. Any new recording-specific evidence can be reviewed against the qualification criteria. If it remains incomplete, the deadline record consists of the verified indoor comparison and the outdoor evidence decisions.
