# Build log: prompts, problems and fixes

Evidence note: This is a retrospective log of work visible in the conversation. Session order is preserved without inventing dates, prompts, feature-development sessions, or test results that were not recorded.

| Session / prompt | What worked | Problem or limitation / response |
| --- | --- | --- |
| 1. “Deploy Deadline Rescue as a public ChatGPT Site and give me the live URL” | Uploaded single-file app was checked, packaged and published; public access was confirmed. | The project needed Site registration and hosting configuration. Deployment succeeded. JavaScript syntax checking passed. |
| 2. “add voiceover to the video about this topic” | English narration was added to the supplied screen recording and synchronized to the visible feature sections. | The uploaded MP4 had no audio stream. A synthesized narration track was created; final audio/video streams were verified. Duration was about 2:08. |
| 3. “i created a repo connect it” plus the repository URL | The repository was reachable and initially contained a README. | GitHub write access was not connected. The user connected GitHub before website upload. |
| 4. Continue after GitHub connection | The deployed index.html and README were committed to main. The uploaded HTML was fetched and matched against the submitted source. | Source backup succeeded. Automatic deployment from GitHub to ChatGPT Sites was not configured. |
| 5. “I want these things for my assignment” and “add this link in the pdf” | This pack brings together links, brief, implementation plan, build log and feature checklist. | The original pre-build plan and feature-by-feature log were not available; these sections are explicitly retrospective. |

## Verified repository history

| Commit | Recorded change |
| --- | --- |
| 1e2cc9b | Initial commit |
| eeb4edf | Add deployed Deadline Rescue student dashboard |
| 4978db7 | Document Deadline Rescue features and live site |

These are real commits observed on the repository. They show setup, source upload and documentation, not a complete feature-by-feature build history. Do not backdate or split work artificially to imitate regular development commits; record future changes as they happen.

## Prompt for the next genuine test session

“Review Deadline Rescue against the core journey. List any reproducible failures, propose the smallest fix for each, and explain the changed code in plain language. Do not add features.” Record the actual response, what you tested and the resulting fix in your next log entry.
