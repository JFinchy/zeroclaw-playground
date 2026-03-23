---
name: metabolic-performance
description: High-performance metabolic tracking for reaching 10% body fat. Use for macro logging (protein-priority), fasting windows, and supplement compliance.
---

# Metabolic Performance Skill (The "10% Shred" Protocol)

This skill is designed to provide ZeroClaw with the specialized logic needed to help Jake reach **10% body fat**. It integrates caloric tracking (input), fasting timing (metabolic state), and supplement compliance (optimal health).

## Core Workflows

### 1. Macro Logging (The "Protein-First" Rule)
Jake's priority is high protein to maintain muscle mass while in a caloric deficit.
- **Trigger:** "Log [food/meal]" or "I just ate [meal]."
- **Action:**
    - Parse the meal for estimated calories and macros.
    - **Highlight Protein:** Always report the protein count immediately.
    - **Deficit Tracker:** Compare current calories against the daily goal (TDEE - 500-750 kcal for fat loss).
- **Format:** Log to `memory/health/YYYY-MM-DD-macros.md`.

### 2. Fasting Window Management
Optimize hormonal balance and fat oxidation through timing.
- **Trigger:** "Start fast," "Break fast," or "Fasting status."
- **Action:**
    - Log start/end times.
    - **Metabolic Phases:** Notify Jake of milestones (12h: Ketosis start, 16h: Fat oxidation peak, 24h: Autophagy).
- **Goal:** Aim for a 16:8 or 18:6 window to support the 10% BF goal.

### 3. Daily Supplement Checklist
Ensure daily micronutrient and performance supplement compliance.
- **Trigger:** "Check my supps," "Morning routine," or "I took my vitamins."
- **Action:**
    - Maintain a checklist in `TOOLS.md` or a daily log.
    - **Reminders:** Proactively ask if supps were taken during morning/evening check-ins.

### 4. The "Road to 10%" Progress Tracker
Weekly metrics to monitor body fat reduction.
- **Action:** Every Sunday, prompt Jake for a weight and body fat % (estimated or measured).
- **Analytics:** Calculate the "weekly delta" and adjust the daily calorie/protein targets if progress stalls.

## Protocol for ZeroClaw

- **High Friction Warnings:** If Jake logs low protein or high sugar/ultra-processed foods, mention the impact on the 10% BF goal (e.g., "Protein is low for this meal; you'll need ~[X]g more today to stay on track").
- **Fasting Alerts:** If Jake is about to eat outside the window, remind him of the current fasting phase.
- **Memory tags:**
    - `#metabolic-fast`: For fasting starts/ends.
    - `#metabolic-protein`: For high protein wins.
    - `#metabolic-supps`: For supplement completion.

## Example Interaction
**Jake:** "I just had a double cheeseburger with no bun and a salad."
**ZeroClaw:** "Logged. Estimated: 650 kcal, **45g Protein**, 35g Fat, 8g Carbs.
Total Protein today: 110g / Goal: 180g.
You've been fasting for 0h since this meal. Fasting timer started.
Did you take your daily supplements yet?"
