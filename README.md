# GTA6Central — Free Video Clip Bot

A free GitHub Actions experiment for downloading a **publicly accessible** video and making a short TikTok-format MP4 for manual review. Uses `yt-dlp` and `FFmpeg`. **Does not publish or upload to TikTok or PostFast.**

## First test (from your phone)

1. Open [Run the GTA6Central video test](https://github.com/BornXrp/gta6central-clipbot/actions/workflows/create-gta6-clip.yml).
2. If GitHub asks you to enable Actions, enable them for this repository.
3. Tap **Run workflow**. Leave the existing public GTA VI video URL, start `0` and duration `20` for the first test.
4. After the run finishes, open its details. Look for a green checkmark (success) or a red X (failure). If it fails, open the **Download and edit a real video** job step to see the actual error.
5. A successful run provides an Actions **artifact** named `gta6-clip-and-report` containing the video and report. The rendered file is a **test clip**, not a published post.

## Rules

- No paid video services, no vidIQ credits, no streamer facecams preferred for current selection.
- Use moving footage. Aim for 15–30 seconds; no one-second clips padded with loops.
- Text should not cover the middle of the game footage (this first basic test doesn't add any overlay).
- Public YouTube/TikTok/Instagram links may be technically blocked by the platforms; success depends on extractor availability.
- Do not use private or DRM-protected sources; only publish material you are entitled to use.
- GitHub Actions artifacts and logs in a public repository may be visible to others. Never add passwords or PostFast API keys in workflow inputs or repository files.
- **There is currently no PostFast integration in the deployed workflow.** Connecting PostFast requires a separate, secure API key setup after the video download tests work.

## Current deployment status

- Repository and Actions workflow installed.
- Local editor prototype's five Python tests passed in the ChatGPT container using generated test footage.
- Remote YouTube download and GitHub Actions workflow **not yet verified by an executed run**.
- No TikTok post has been made by this bot.
