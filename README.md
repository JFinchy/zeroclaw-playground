# Jake's Personal ZeroClaw OS

This repository contains my personal configuration and custom skills for [ZeroClaw](https://github.com/openclaw/zeroclaw), an interactive CLI agent and personal operating system.

## 🧠 Core Architecture

My ZeroClaw setup acts as an external brain, maintaining continuity across sessions using local file storage. It handles everything from automating business ideation to managing my golf game.

### Included Skills

This workspace is loaded with several custom skills tailored to my life:

*   **`golf-reservation`**: The "Solo Golf Scout". A headless scraper that monitors local Roseville/Placer County courses (Woodcreek, Diamond Oaks, Sun City, etc.) to find and alert me of "Blocks of Air" (3+ open slots) so I can play cheap, solo twilight rounds without getting paired up.
*   **`golf-pro`**: A digital caddie that tracks my club yardages, round stats, and logs my swing thoughts.
*   **`tax-professional`**: A proactive tax advisor that categorizes my expenses, alerts me of quarterly estimated deadlines, and optimizes deductions across mixed W-2/1099 income.
*   **`card-optimizer`**: Tracks credit card 5/24 status, sign-up bonus minimum spend deadlines, and tells me exactly which card to swipe for maximum ROI on specific purchases.
*   **`health-officer`**: A central hub that correlates my bloodwork, sleep data, and gym PRs, adjusting my macros on the fly if I log an injury.
*   **`fleet-manager`**: Uses cron jobs to proactively remind me about vehicle maintenance (oil, tires) and home upkeep (HVAC filters, water heaters) before things break.
*   **`personal-crm`**: A network maintainer that logs details from coffee meetups and nudges me to reach out to friends who have fallen off the radar.
*   **`slow-burn-researcher`**: An asynchronous agent that deep-dives into topics over weeks, builds taxonomies, and generates Anki flashcards for knowledge retention.
*   **`relationship-skills`**: Frameworks for conflict resolution and connection building.
*   **`crucial-conversations-coach`**: An executive coach designed to help navigate high-stakes, emotional discussions.
*   **`anki-connect`**: Integrates with Anki for automated flashcard generation.
*   **`product-ideation`**: An autonomous 4-stage pipeline that generates weird, profitable business models via forced lateral connections.

## 🔒 Security

All API keys and secrets in the `config.toml` are locally encrypted using ZeroClaw's `enc2:` protocol. The `.secret_key` required to decrypt them, along with all personal data logs in `workspace/data/`, are strictly ignored via `.gitignore`.
