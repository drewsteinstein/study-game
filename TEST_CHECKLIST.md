# First-Open and Regression Checklist

Status: planned checklist; not yet executed against the repository's imported source.

## Import and baseline
- [ ] Import the exact v0.1.1 source from the preserved Dropbox archive.
- [ ] Record source archive name and checksum.
- [ ] Preserve v0.1 and v0.1.1 archives outside any destructive edit.
- [ ] Review the source diff against the previous baseline.

## Automated checks
- [ ] `node --check core.js`
- [ ] `node --check app.js`
- [ ] `node --test tests/core.test.cjs` — expected baseline: 10 passed, 0 failed.
- [ ] Verify archive or source package integrity.

## Real-browser flow
- [ ] Open the extracted `index.html` in Chrome or another supported browser.
- [ ] Start and complete a 5-question flight.
- [ ] Confirm answers, feedback, explanations, and seed rewards are correct.
- [ ] Re-answer a seen card and confirm rewards cannot be farmed.
- [ ] Purchase a bird; confirm insufficient funds and duplicate adoption behave correctly.
- [ ] Complete the full course and verify the 9/12 invitation threshold.
- [ ] Check navigation and Progress metrics.
- [ ] Refresh and restart browser; confirm state persists when storage is available.
- [ ] Test a clean save, malformed save, and storage-blocked browser.
- [ ] Confirm accuracy never exceeds 100%.
- [ ] Inspect console for errors and test a narrow mobile viewport for overflow.

## Acceptance bar
Do not call the baseline release-ready until the automated checks pass and the real-browser smoke tests are completed. If a check cannot be run, record the blocker explicitly rather than marking it passed.
