# Song Finder

AI 101 midterm project, Alvernia University.

## Audience
Anyone who loves music or keeps hunting for new songs, especially people who are getting bored of the same playlist.

## Purpose
Playlists get repetitive. Song Finder takes a few songs or artists you like, works out which genre they belong to, and suggests other songs from that genre with a link to listen on your streaming platform.

## First two features
1. **Genre detection:** type songs or artists separated by commas, and the app matches them to a genre.
2. **Recommendations with links:** the app shows songs from the detected genre (skipping what you typed) with a Listen link for Spotify, YouTube Music, or Apple Music. A row of genre buttons works as a fallback when a song isn't in the sample data.

## How to run it
No install needed. Download `index.html` and open it in any browser. To test, type `Blinding Lights, Levitating` and press **Find songs**.

## Current progress
**Works:** genre detection from the sample data, recommendations that skip your input, platform links, genre buttons, empty and unknown input handled without crashing.

**Not done yet (planned for the final):**
- Real AI genre detection for songs outside the sample data. The sample data has 5 genres and 40 songs.
- Saving lists between visits (browser storage first).
- More genres and more streaming platforms.

## AI assistance
Claude (Anthropic) generated the code, the sample song data, this README, and the agent instructions in `CLAUDE.md`. I directed the project idea, scope, and features.

**What I verified myself:** see the proof checks below.

## Issue #1: Recommend songs from the detected genre
**Acceptance criteria**
- Given 2 Pop songs, the app shows 6 other Pop songs and none of the 2 I typed.
- Given an artist and a song from different genres, the app shows both genres.
- Given text that isn't in the data, the app shows a "not in the sample data" message instead of crashing.
- Every result has a Listen link that opens a search for that song on the chosen platform.

## Proof checks (to be completed by me)
Fill in what actually happened when you ran each test.

| Test | Expected | What actually happened |
|---|---|---|
| `Blinding Lights, Levitating` | Pop, 6 results | |
| `Kendrick Lamar, Mr. Brightside` | Hip-Hop and Rock, no Kendrick results | |
| `asdfgh` | "Not in the sample data" message, no crash | |
| Click a Listen link (all 3 platforms) | Search opens for the right song | |
| Spot-check 10 songs in the sample data | Each song really exists by that artist | |

**Challenge I want help with:** can AI power the recommendations without paying for an always-running agent?
