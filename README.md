# JerinexBotNavigation 2.0 — source recovery starter

This ZIP contains the uploaded 1.0.0 JAR and a GitHub Actions workflow starter.

## Requested behavior to implement

- Levers: randomized 2–5 tick delay.
- Any wool block: randomized 2–5 tick delay.
- Nether wart block: randomized 2–5 tick delay.
- Any button: randomized 2–5 tick delay.
- Cobweb: randomized 2–5 tick delay ONLY when cobweb is in the offhand.
- Cobweb in main hand: vanilla/normal placement.
- Any unrelated item/block: vanilla/normal placement.
- Shield-stun behavior stays unchanged: after a shield disable is detected, wait exactly 2 ticks, then issue one attack against the same valid target.

## Important limitation

The upload was a compiled JAR, not the original Gradle source project. This starter preserves the original JAR, but it does **not** contain reconstructed Java source or the requested delay fix. The workflow below only packages the original JAR as an artifact; it does not pretend to compile a modified 2.0 mod.

To produce a real fixed build, add the original project source (`build.gradle`, `settings.gradle`, `gradle.properties`, `src/`) and implement the behavior above. Do not upload this starter artifact as if it were the fixed mod.
