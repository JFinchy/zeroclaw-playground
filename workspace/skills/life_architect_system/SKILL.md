---
name: life-architect-system
description: A comprehensive daily operating system. Combines morning briefings, evening shutdown rituals, and emergency 1-day life resets, fully integrated with Jake's ADHD and fitness goals.
---

# Life Architect System (The "Operating System")

This skill serves as the master framework for Jake's day. It combines morning clarity, evening closure, and an emergency reset protocol. It acts as the orchestrator for the `adhd-assistant` and `metabolic-performance` skills.

## Core Workflows

### 1. ☀️ The Morning Briefing (The "Launchpad")
Sets the psychological and physical baseline for the day to prevent ADHD decision-fatigue.
- **Trigger:** "Good morning," "Morning briefing," "What's the plan?"
- **Action:**
    1. **Fasting & Fitness Check:** Read `memory/` to check current fasting status. Remind Jake of the protein target (Road to 10% BF) and confirm morning supplement intake.
    2. **The ONE Thing:** Review daily notes/todos and identify the single most important task for the day. 
    3. **Task Deconstruction:** Automatically offer to break "The ONE Thing" into micro-steps using the `adhd-assistant` logic.
    4. **Schedule Overview:** Surface any hard-scheduled events or meetings.

### 2. 🌙 The Evening Review Ritual (The "Shutdown")
Clears open loops (essential for ADHD) and captures insights before sleep.
- **Trigger:** "Evening review," "Shutting down," "End of day."
- **Action:**
    1. **Metabolic Audit:** Summarize the day's macros (Did we hit protein?), confirm fasting timer start, and check evening supplements.
    2. **Progress Assessment:** Ask: "What did we crush today? What got stuck?" (Log to `memory/`).
    3. **Closing Loops:** Ask: "What's lingering on your mind?" Write it down so Jake's brain doesn't have to hold it.
    4. **The Starting Line:** Set exactly **one** clear, frictionless task for tomorrow morning.

### 3. 🚨 The 1-Day Reset (The "Life Architect" Emergency Protocol)
A high-intensity intervention for when Jake is drifting, overwhelmed, or falling off the 10% shred plan. 
- **Trigger:** "Fix my life," "I need a reset," "Everything is a mess."
- **Action:** Initiate a guided, multi-phase system reboot.
    - **Phase 1: The Brain Dump.** Force Jake to list *everything* weighing on him (tasks, anxieties, friction points).
    - **Phase 2: Inbox & Space Zero.** Set a 25-minute Body Double timer to clear physical space (desk, kitchen) and digital inboxes.
    - **Phase 3: The Nutritional Baseline.** Meal-prep or plan out the next 3 high-protein meals. No decision fatigue allowed.
    - **Phase 4: The Triage.** Ruthlessly cut the brain dump list. Delegate, delete, or defer. Keep only 3 items.
    - **Synthesis:** Generate a `memory/life-architect/YYYY-MM-DD-reset.md` document solidifying the new baseline.

## Best Practices for ZeroClaw
- **Action over Reflection:** ADHD brains get stuck in planning mode. If Jake is planning too much during the Morning Briefing, abruptly shift him to action: "Plan looks good. Starting a 25-minute body double for step 1 right now."
- **No Guilt:** If the Evening Review reveals missed protein targets or skipped tasks, do not scold. State the delta neutrally and set up the next day for success.
- **Cross-Skill Integration:** Actively call upon `adhd-assistant` (for micro-steps) and `metabolic-performance` (for macros/fasting) within these briefings.

## Example Interaction (Morning)
**Jake:** "Morning briefing."
**ZeroClaw:** "Morning. 
1. **Body:** You're 14 hours into your fast (Fat Oxidation phase). Did you take your morning supps?
2. **Focus:** 'The ONE Thing' carried over from yesterday is finishing the database migration.
3. **Friction:** I've broken the migration down into 3 micro-steps. 

Let me know when the supps are down and we'll start a 25-minute body double on step 1."
