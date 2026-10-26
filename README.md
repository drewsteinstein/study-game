# Feather & Field — Bird Sanctuary Study Game

A prototype that combines active-recall study with building and discovering a bird sanctuary.

## Current baseline

The current known-good prototype is **v0.1.1 accuracy fix**, maintained in the project's Dropbox handoff. The original v0.1 package is preserved separately. This repository is the intended code home, but the source package has not yet been imported here.

## What is known to work

The v0.1.1 patch corrected a saved-progress accuracy bug: malformed state could show more correct answers than total answers (for example, 9/1 = 900%). State normalization now caps correct answers at total answers.

The accompanying report says these checks passed:
- `node --check core.js`
- `node --check app.js`
- `node --test tests/core.test.cjs` (10 passed, 0 failed)
- ZIP integrity check

**Not yet verified:** first-open browser behavior for the packaged game. The prior test environment blocked local browser navigation, so browser behavior must still be checked manually.

## Product direction

The intended experience is a useful study tool first, with a sanctuary-building/discovery loop that reinforces learning rather than distracting from it. The prototype is not yet a validated final design.

Priorities:
1. Import the exact v0.1.1 source without overwriting the original baseline.
2. Establish repeatable tests and a browser smoke-test checklist.
3. Verify question accuracy, answer feedback, rewards, save/reload, and malformed/missing saved data.
4. Evaluate whether the sanctuary loop improves motivation without slowing down study.
5. Add features only when they improve learning, usability, or reliability.

## Development rules

- Keep changes small and reviewable.
- Preserve known-good versions and saved progress.
- Test actual user journeys, not just syntax.
- Turn discovered bugs into regression tests.
- Clearly distinguish executed tests from manual checks that have not been performed.
- Do not treat prototype rewards, prices, or unlock thresholds as user-approved conclusions.

## Status

This repository was created as the planned GitHub home. The actual game source and historical handoff materials still need to be imported and checked against the preserved Dropbox originals.
