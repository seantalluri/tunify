# Audio Quality and Confidence Policy

## AQ-01 — Hard stop for unusable input

Stop and request a new recording when the file is corrupted, no melody is detected, or noise prevents recovery of a meaningful pitch contour. Do not produce an arrangement recommendation.

## AQ-02 — Proceed at high confidence

When both tempo and key confidence are 80% or higher and the file is valid, proceed without unnecessary clarification.

## AQ-03 — Clarify below 60%

When either tempo or key confidence is below 60% but a meaningful pitch contour remains, strongly recommend re-recording and explain the uncertainty. The singer may choose **Continue anyway**; if so, label uncertain assumptions in every result.

## AQ-04 — Confirm from 60% through 79%

When either tempo or key confidence is from 60% through 79%, present the likely values and ask the singer to confirm before continuing.

## AQ-05 — Missing required context

When a required melody, style, structure, chord, instrument, rights, or policy record is missing, stop and name the missing record. Ask the singer to provide it or escalate. Never invent a replacement value.
