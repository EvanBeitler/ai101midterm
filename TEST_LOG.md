# Test Log
Run every test on the **live GitHub Pages site** (private window). Fill in Actual and Result yourself, honestly.

| # | Test | Steps | Expected | Actual | Pass/Fail |
|---|------|-------|----------|--------|-----------|
| 1 | Normal input | Type `Blinding Lights, Levitating`, press Find songs | Genre Pop, 6 songs, neither typed song listed | Pop, 6 songs, neither duplicates | Pass |
| 2 | Empty / invalid | Press Find songs with an empty box, then try `asdfgh` | No crash; empty box shows a no-matches message; `asdfgh` is listed as not in the sample data | 'asdfgh' is not listed in the sample data | Pass |
| 3 | Repeated use | Search 3 times in a row with different inputs, change platform, click genre buttons | Results replace the old ones each time; links change to the chosen platform | Does replace old ones each time | Pass |
| 4 | Keyboard access | Use only Tab, Enter and Shift+Tab to search and open a Listen link | Every control is reachable, focus outline is visible, Enter runs a search | Works as intended | Pass |
| 5 | Narrow screen | Open on your phone (or shrink the window below 600px) | Single column, search box first, no sideways scrolling | Works as intended | Pass |

## Fact check
Spot-check about 10 songs from the sample data against an official source (Spotify or the artist's page). Note any wrong ones: ______

## One fix and retest
- Problem found: ______
- Fix (prompt or change): ______
- Retest result: ______
