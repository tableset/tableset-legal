# Hosting Events Screenshots — Checklist

Capture these in the iOS Simulator (iPhone 17 Pro) and save to `screenshots/` in this repo. Use the same naming convention as existing files (e.g., `12a-event-wizard-day.png`).

**Setup before capturing**: Create a Summer BBQ event in your simulator with realistic data so the screenshots look polished. You'll need:
- An event named "Summer BBQ" (or similar) for ~12 guests
- 2-3 prep days selected
- A few dishes generated (Mains, Sides, Desserts)
- 2-3 contributors added

---

## Required Screenshots (9 total)

### 1. `12a-event-wizard-day.png`
**Where in the app**: Plan tab → wand icon → "Plan Event" → Step 1 (Pick a Day)
**What to capture**: The full wizard step showing the 7-day picker. **Make sure at least one day has an existing event** so the disabled/grayed-out state is visible (proves the "one event per day" rule).
**Used for**: Section 10 → "Creating an Event"

### 2. `12b-event-wizard-prep.png`
**Where in the app**: Same wizard → Step 5 (Prep Availability)
**What to capture**: The calendar grid with 2-3 prep days selected (event day + 1-2 days before). Below the grid, show one day expanded with the "Time windows" mode active so the start/end pickers and total hours are visible.
**Used for**: Section 10 → "Creating an Event" (highlights the unique calendar+windows UX)

### 3. `12c-event-wizard-scope.png`
**Where in the app**: Same wizard → Step 6 (AI Planning Scope)
**What to capture**: The three scope cards: "Plan whole menu", "Plan specific sections", "I'll plan it myself". Tap "Plan whole menu" so it shows as selected.
**Used for**: Section 10 → "Creating an Event"

### 4. `12d-event-menu.png`
**Where in the app**: After completing the wizard and AI generation finishes → the event view's **Menu** tab
**What to capture**: The full Menu tab with the event header (stats), the segmented tab picker, and at least 2-3 dish cards visible across multiple categories (e.g., Mains and Sides). **Make sure dish cards have images** (wait for image generation).
**Used for**: Section 10 → "The Event View"

### 5. `12e-event-dish-card.png`
**Where in the app**: Same Menu tab — capture a close-up of ONE rich dish card
**What to capture**: Crop or scroll so a single dish card fills most of the frame. The card should show: 72x72 image, dish title, cuisine/time/difficulty badges, contributor avatar, status badge, prep timing.
**Used for**: Section 10 → "Adding Dishes" (or could move to "The Event View")

### 6. `12f-event-timeline.png`
**Where in the app**: Event view → **Timeline** tab (after tapping "Generate Timeline")
**What to capture**: The full Timeline tab showing:
- The progress header
- The horizontal **phase pills** (e.g., "1 Day Before", "Day Of") with one selected
- The **"Start at:" time picker** below the pills
- 3-4 step rows with the colored dots, clock time badges (e.g., "9:30 AM"), task titles, dish names, and durations

**Used for**: Section 10 → "Cooking Timeline"

### 7. `12g-activity-view.png`
**Where in the app**: Tap any timeline step → tap "Start Activity"
**What to capture**: The fullscreen activity view showing:
- The progress bar at top ("Step 2 of 5")
- A clear instruction sentence (e.g., "Whisk dry ingredients in a large bowl")
- The timer card (Start Timer button visible)
- The "Ingredients for this step" card with 3-4 ingredients
- Previous/Next buttons at the bottom

**Used for**: Section 10 → "The Activity View"

### 8. `12h-event-shopping.png`
**Where in the app**: Event view → **Shopping** tab
**What to capture**: The aggregated grocery list grouped by category (produce, proteins, etc.).
**Used for**: Section 10 → "Shopping List"

### 9. `12i-day-card-event.png`
**Where in the app**: Plan tab — view the week containing your event
**What to capture**: ONE day card that has a hosting event on it. Should show the rich event gateway card with:
- Party-popper icon and event name
- "11 dishes" badge in the top-right corner
- Contributor avatars row
- Status counts ("11 confirmed" etc.)
- "Tap to view full menu" hint
- The "..." menu icon visible

**Used for**: Section 10 → could go in "The Event View" or as the very first screenshot of the section

---

## Optional Bonus Screenshots

### `12j-step-detail-summary.png` (optional)
The intermediate "Step Detail" view (between tapping a row and tapping Start Activity) — shows the summary card and the big green "Start Activity" button.

### `12k-must-make-toggle.png` (optional)
A dish card with the "Must-make" star showing.

---

## How to Capture in iOS Simulator

1. Run the app on the simulator (iPhone 17 Pro recommended for crisp screenshots)
2. Navigate to the screen described above
3. Press **⌘ + S** in the simulator (or Hardware → Save Screen)
4. Screenshots save to your Desktop
5. Rename to the filename above and drop into `~/Documents/PROJECTS/tableset-legal/screenshots/`

## When You're Done

Tell Claude "I added the screenshots" and provide the list of filenames you saved. Claude will then:
1. Verify each file exists
2. Insert the `<div class="screenshot">` blocks at the right positions in `guide.html`
3. Match the existing styling (single image or paired layout)
4. Commit and push everything together

---

## Notes

- **Don't worry about pixel-perfect**: the existing screenshots are unstyled simulator captures. Match that.
- **Light mode preferred** for consistency with the existing screenshots.
- **Hide your real name**: if your simulator shows "Corey" anywhere, sign in as the Dev User or use "Sarah" to match the Smith family example.
- If a screenshot turns out hard to capture (e.g., AI generation hasn't finished), skip it and tell Claude — we can still add the rest.
