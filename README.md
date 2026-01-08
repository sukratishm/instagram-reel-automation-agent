Instagram Reel Automation

Automated faceless Instagram Reel creation and publishing using a local n8n instance and Blotato.

This workflow runs end-to-end without manual intervention:
idea selection → script & caption generation → video creation → Instagram publishing.

If you like automations that work while you sleep, this one’s caffeinated ☕

Why this exists

Posting Reels consistently is hard.
Creating videos is time-consuming.
Doing it daily is… character building.

This automation solves that by:

removing the need to record yourself,

eliminating repetitive manual work,

ensuring ideas are not reused,

publishing content on autopilot.

Once configured, the workflow can run 24/7 on a local n8n instance.

What this automation does (high level)

Triggers on a schedule

Fetches previously used content ideas

Generates a new script + caption

Sends content to Blotato to generate a video

Uploads the video to Instagram

Marks the idea as “used” to avoid repetition

No dashboards. No uploads. No clicking buttons like a caveman.

Tech stack

n8n (self-hosted / local instance)

Blotato API (video creation + Instagram publishing)

Optional: AI model credentials used inside n8n (e.g. OpenAI)
