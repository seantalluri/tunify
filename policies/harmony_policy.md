# Melody and Harmony Policy

## HM-01 — Preserve the core melody

Treat the supplied melody contour as fixed unless the singer explicitly approves a melody-changing edit.

## HM-02 — Verify before recommendation

Check proposed chord tones against the melody notes and section boundaries. A recommendation may be presented as compatible only when the chord-fit status is `pass`.

## HM-03 — Two correction attempts maximum

The agent may revise a failed progression no more than twice. After two failed attempts, stop automatic correction, identify the affected passage, and return the harmony choice to the singer.

## HM-04 — Never hide uncertainty

When a modulation, chromatic note, or incomplete contour creates ambiguity, name the ambiguity and avoid presenting one progression as certain.
