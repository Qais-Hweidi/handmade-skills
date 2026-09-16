---
name: debug
description: Investigate bugs and unexpected behavior, establish the root cause, and verify a fix.
---

# Debug

Establish the observed behavior, expected behavior, and conditions of the failure. Reproduce it when possible.

Identify the evidence needed to investigate the failure across the relevant components. Do not limit the investigation to whichever sources are easiest to access.

If relevant evidence cannot be obtained, stop and tell the user what is unavailable, why, how it limits the investigation, and what is needed to proceed. Wait for the evidence, restored access, or explicit direction from the user before continuing.

Never treat inaccessible evidence as evidence that a component is healthy. Keep observations, hypotheses, and confirmed causes distinct.

Test hypotheses with focused checks that distinguish between plausible causes. Before implementing any fix, establish the root cause with supporting evidence. A plausible explanation alone is not enough.

Once the root cause is established, make a targeted fix within the requested scope. Verify against the original failure and relevant checks.

If a fix does not fully resolve the issue, reassess the diagnosis and the change before adding another fix. Keep the change only if evidence shows it addresses a confirmed part of the problem; otherwise, revert that attempted fix without disturbing unrelated work. Investigate what remains instead of stacking speculative changes.

Report the evidence supporting the diagnosis, what changed, verification results, and any remaining uncertainty.
