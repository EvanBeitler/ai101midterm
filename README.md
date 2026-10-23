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


**Challenge I want help with:** can AI power the recommendations without paying for an always-running agent?
