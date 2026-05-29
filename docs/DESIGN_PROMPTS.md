# Design Prompts

This document keeps track of the prompts used to generate UI/UX designs for the Budget Tracker app.

## User Feedback (Mid-exploration Pivot)
*   **Feedback on Prompt #2 (Neobrutalism / Playful):** The playful and interesting mood was highly appreciated. However, the high-contrast pastel colors were too bright and harsh on the eyes, especially for nighttime use.
*   **Feedback on Prompt #3 (Zen / Glassmorphism):** While clean and beautiful, the overall look felt too common, generic, and slightly boring.
*   **The Pivot:** A request for a "middle ground" that blends the fun, quirky elements of Neobrutalism with a dark, subtle, low-contrast palette that is easy on the eyes. Prompts #4 and #5 explore this direction.

## Prompt #1: Industry Standard (Clean & Minimal)

**Goal:** Create a clean, minimal, industry-standard mobile UI that is highly functional but safe.

```text
Design a mobile-first UI for a daily budget tracking web app. The primary goal is for users to see if they are within budget for the day and to log transactions as fast as possible. The design should follow standard iOS/Android mobile web patterns, feel modern but simple, and use a standard utility-like color palette (using shadcn/ui components styling).

Please generate the following 3 core mobile screens:

1. **Home Summary Screen (The Dashboard)**
- **Header:** Today's Date.
- **Hero Metric:** A large, clear typography showing "Remaining Budget Today". Use color dynamically (e.g., green for healthy, orange for close to limit, red for over budget).
- **Secondary Metrics (smaller text below):** "Total Income: X" and "Total Expense: Y".
- **Visual Indicator:** A simple horizontal progress bar showing how much of the daily budget has been spent.
- **Recent Activity:** A short list of the 3 most recent transactions today.
- **Primary Action:** A floating action button (FAB) or a large fixed bottom button saying "Add Transaction" positioned for easy 1-thumb reach.

2. **Add Transaction Screen (Bottom Sheet or Modal)**
- **Format:** Should look like a slide-up bottom sheet over the Home Screen.
- **Inputs:**
  - A segmented control or toggle for "Income / Expense" (Default to Expense).
  - A large number pad or simple large input field for the "Amount".
  - A grid or horizontal scroll of "Quick Select Categories" (e.g., Food, Transport, Coffee) with simple icons.
  - An optional, single-line text input for "Short Note".
- **Action:** A prominent "Save" button at the bottom.

3. **History List Screen**
- **Header:** "Today's Transactions".
- **List:** A full-page scrollable list of today's logged items. Each row should show the Category Icon, Short Note, Time, and Amount (green for income, red for expense).
- **Interaction:** Indicate that rows can be swiped to Edit/Delete.
- **Bottom Navigation:** A simple bottom nav bar to switch between "Home" and "History".

**Design Constraints:**
- Prioritize "1-thumb usage" (interactive elements should be in the lower half of the screen).
- Fast input: use preset visual chips for categories instead of long dropdown menus.
- Zero-confusion copy: Keep text very brief and focused.
- Clean, minimal aesthetic. Empty states should have a friendly prompt to add the first transaction.
```

## Prompt #2: Neobrutalism / Playful

**Goal:** Stand out from boring banking apps by using bold, high-contrast, playful styling while maintaining a simple mobile UX.

```text
Design a mobile-first UI for a daily budget tracking web app. Maintain standard mobile UX layouts, but completely replace the visual styling with a "Neobrutalist / Playful" aesthetic.

Visual Style Guidelines:
- Use bold, high-contrast pastel colors (e.g., retro yellow, punchy pink, mint green).
- UI elements (cards, buttons, inputs) should have thick black borders and sharp, flat drop shadows.
- Typography should be bold, slightly quirky, and highly legible.
- The vibe should feel like a fun game or a cool modern indie app (similar to Gumroad or Figma's playful style), NOT a boring banking app.

Please generate the following 3 core mobile screens:

1. **Home Summary Screen (The Dashboard)**
- **Header:** Today's Date.
- **Hero Metric:** A massive, punchy typography showing "Remaining Budget Today". Use bold background colors on this card to indicate health (Green for good, Orange for warning, Red for over).
- **Secondary Metrics:** "Total Income" and "Total Expense" in chunky, bordered boxes.
- **Visual Indicator:** A thick, chunky progress bar.
- **Recent Activity:** A list of 3 recent transactions. Each item should be its own bordered card.
- **Primary Action:** A massive, thick-bordered "Add Transaction" button at the bottom.

2. **Add Transaction Screen (Bottom Sheet)**
- **Format:** A slide-up bottom sheet with a thick black border at the top edge.
- **Inputs:**
  - A chunky toggle switch for "Income / Expense".
  - A giant, playful number pad for the "Amount".
  - "Quick Select Categories" as colorful, bordered pill buttons with bold icons.
- **Action:** A giant, brightly colored "Save" button.

3. **History List Screen**
- **Header:** "Today's Log".
- **List:** Scrollable list. Each transaction is a bold card with high contrast text.
- **Bottom Navigation:** A chunky bottom nav bar with distinct, bold icons.
```

## Prompt #3: Zen / Glassmorphism

**Goal:** Create a premium, calming atmosphere to reduce financial anxiety, focusing on soft gradients and breathing room.

```text
Design a mobile-first UI for a daily budget tracking web app. Maintain standard mobile UX layouts, but style the app using a "Zen / Glassmorphism" aesthetic to make budgeting feel calming and stress-free.

Visual Style Guidelines:
- Use a dark mode theme (deep slate, midnight blue, or absolute black) OR a very soft, airy light mode.
- Use Glassmorphism heavily: translucent panels, background blur, and soft, ethereal gradients that bleed softly into the background.
- Typography should be elegant, thin, and spacious.
- Remove harsh borders entirely. Use soft glows and shadows to separate elements.
- The vibe should feel like a premium mindfulness or wellness app (like Headspace or Calm).

Please generate the following 3 core mobile screens:

1. **Home Summary Screen (The Dashboard)**
- **Header:** Today's Date in elegant, quiet text.
- **Hero Metric:** "Remaining Budget Today" should be large but ethereal, perhaps with a soft glowing background gradient that changes color based on health (soft emerald glow for good, soft crimson glow for over budget).
- **Secondary Metrics:** "Income" and "Expense" floating gently on translucent glass cards.
- **Visual Indicator:** A very thin, elegant ring chart or smooth, soft progress line.
- **Recent Activity:** A list of the 3 recent transactions fading softly at the edges.
- **Primary Action:** A floating, translucent glass button with a soft glow for "Add Transaction".

2. **Add Transaction Screen (Bottom Sheet)**
- **Format:** A slide-up glass panel blurring the Home Screen behind it.
- **Inputs:**
  - A sleek, minimalist toggle for "Income / Expense".
  - A large, thin-font number pad for the "Amount".
  - "Quick Select Categories" floating softly as subtle icons without harsh borders.
- **Action:** A softly glowing "Save" button.

3. **History List Screen**
- **Header:** "Today".
- **List:** Scrollable list. Items should feel like they are floating on the glass background.
- **Bottom Navigation:** A translucent glass bottom nav bar.
```

## Prompt #4: Soft Dark Neobrutalism

**Goal:** Find a "middle ground" by keeping the playful, thick-bordered aesthetic of Neobrutalism, but adapting it for a muted, low-contrast dark mode to be easy on the eyes.

```text
Design a mobile-first UI for a daily budget tracking web app. Maintain standard mobile UX layouts, but style the app using a "Soft Dark Neobrutalism" aesthetic. The goal is to blend the fun, quirky layout of Neobrutalism with a relaxing, low-contrast dark mode palette.

Visual Style Guidelines:
- **Background Palette:** Use deep, matte colors (e.g., charcoal, soft deep navy, or dark mocha) to keep the screen dark and easy on the eyes.
- **Accent Colors:** Use muted, low-intensity pastel accents (dusty rose, sage green, mustard yellow, muted lavender) rather than high-contrast neons.
- **Borders & Shadows:** Retain the playful thick borders and flat drop shadows on cards and buttons, but instead of harsh black borders, use slightly darker or lighter tonal colors (e.g., a dark grey border on a charcoal background, or soft colored borders).
- **Typography:** Playful, rounded, and bold, but in soft off-white or muted text colors to reduce eye strain.

Please generate the following 3 core mobile screens:

1. **Home Summary Screen (The Dashboard)**
- **Header:** Today's Date in a friendly, chunky font.
- **Hero Metric:** "Remaining Budget Today" inside a rounded, chunky-bordered card. The card's background color is subtle, but indicates health (muted sage for good, muted rust/orange for warning).
- **Secondary Metrics:** "Total Income" and "Total Expense" inside playful, slightly asymmetrical pill-shaped boxes.
- **Visual Indicator:** A thick, rounded progress bar.
- **Recent Activity:** A list of 3 recent transactions. Each item is a dark, rounded card with a soft-colored drop shadow.
- **Primary Action:** A chunky, thick-bordered "Add Transaction" button at the bottom.

2. **Add Transaction Screen (Bottom Sheet)**
- **Format:** A slide-up bottom sheet with a thick, rounded top edge.
- **Inputs:**
  - A chunky toggle switch for "Income / Expense".
  - A large, playful but muted number pad for the "Amount".
  - "Quick Select Categories" as dark pill buttons with soft, colorful icons.
- **Action:** A giant, inviting "Save" button in a muted pastel shade.

3. **History List Screen**
- **Header:** "Today's Log".
- **List:** Scrollable list. Each transaction is a soft-dark card with playful iconography.
- **Bottom Navigation:** A chunky bottom nav bar with friendly, slightly cartoonish icons.
```

## Prompt #5: Bubbly Midnight / Playful Dark

**Goal:** An alternative "middle ground" that replaces harsh borders with soft, bubbly shapes and gentle contrast, maintaining a fun vibe within a relaxing dark mode environment.

```text
Design a mobile-first UI for a daily budget tracking web app. Maintain standard mobile UX layouts, but style the app using a "Bubbly Midnight" aesthetic. The goal is to create a UI that is playful and inviting, but soft, dark, and highly ergonomic for nighttime viewing.

Visual Style Guidelines:
- **Background Palette:** Use a deep, rich midnight-sky palette (deep indigo, twilight blue, dark purple).
- **Shapes & Corners:** Avoid sharp edges and thick borders completely. Everything should be ultra-rounded, soft, and bubbly (squircle shapes, pill forms, cloud-like containers).
- **Colors & Lighting:** Rely on very soft, diffuse inner glows or gentle low-contrast background fills to separate elements. Accent colors should be low-light bio-luminescent tones (soft cyan, glowing lilac, warm muted gold).
- **Typography:** Friendly, rounded sans-serif fonts. Text should be legible but not stark white.

Please generate the following 3 core mobile screens:

1. **Home Summary Screen (The Dashboard)**
- **Header:** Today's Date in a soft, rounded font.
- **Hero Metric:** "Remaining Budget Today" inside a massive, soft, bubbly container. Use a very gentle background glow (soft teal for healthy, soft amber for caution) to indicate status.
- **Secondary Metrics:** "Income" and "Expense" in floating, pill-shaped bubbles.
- **Visual Indicator:** A thick but soft, jelly-like progress bar.
- **Recent Activity:** 3 recent transactions shown as soft, nested bubbles with very subtle color differences from the background.
- **Primary Action:** A pillowy, ultra-rounded FAB or bottom button that looks squishy and inviting.

2. **Add Transaction Screen (Bottom Sheet)**
- **Format:** A slide-up bottom sheet with an extremely rounded, bubbly top edge.
- **Inputs:**
  - A soft, jelly-like toggle for "Income / Expense".
  - A simple, rounded number pad.
  - "Quick Select Categories" as soft circular bubbles with simple, friendly icons.
- **Action:** A large, squishy "Save" button.

3. **History List Screen**
- **Header:** "Today's Log".
- **List:** Scrollable list. Each transaction is a soft bubble row.
- **Bottom Navigation:** An ultra-rounded floating bottom nav bar containing simple, soft-glowing icons.
```

## Prompt #6: Outlined Playful / Modern Flat Illustration (Alegria-inspired)

**Goal:** Emulate a warm, highly illustrative style characterized by flat colors, distinct outlines, playful proportions, and a "sticker-like" feel, moving away from generic UI shapes toward artwork-driven design.

```text
Design a mobile-first UI for a daily budget tracking web app. The core layout should be standard for mobile, but the visual execution MUST heavily feature a specific illustrative style: "Modern Flat Illustration with Outlines" (similar to Corporate Memphis, Alegria, or a refined sticker aesthetic).

Visual Style Guidelines:
- **Heavy Use of Illustration:** The UI should be anchored by prominent, stylized illustrations. Don't just use standard FontAwesome/Material icons; use chunky, custom-looking vector art.
- **Flat Colors & Outlines:** Illustrations and key UI elements (like cards or prominent buttons) should use flat, solid fill colors bordered by distinct, dark (or colored) outlines. This gives a "sticker" or "comic-book" pop.
- **Playful Proportions:** Objects and characters (if any) should be stylized, slightly chunky, and abstract rather than realistic.
- **Warm, Subtle Palette:** Use a soft, warm background color (e.g., pale peach, soft lavender, buttery yellow). Accent colors should be vibrant but slightly desaturated pastel or mid-tones (warm pinks, sky blues, mustard yellows) to maintain a friendly, not harsh, contrast.
- **Subtle Texture:** Add a very light grain or subtle offset drop shadow to the outlined elements to give them slight depth without losing the flat feel.

Please generate the following 3 core mobile screens:

1. **Home Summary Screen (The Dashboard)**
- **Header:** Today's Date.
- **Hero Area:** A large, prominent illustration representing "Budget Health" (e.g., a stylized, outlined piggy bank or a chunky wallet). "Remaining Budget" should be displayed boldly near this illustration.
- **Secondary Metrics:** "Income" and "Expense" displayed on soft-colored cards with subtle outlines.
- **Recent Activity:** A list of 3 recent transactions. Each category icon MUST be a custom, outlined, playful illustration (e.g., a chunky coffee cup, a stylized outline of a car).
- **Primary Action:** A prominent "Add Transaction" button that looks like a pill or rounded rectangle with a distinct outline.

2. **Add Transaction Screen (Bottom Sheet)**
- **Format:** A slide-up bottom sheet.
- **Inputs:**
  - Toggle for "Income / Expense".
  - A clean number pad.
  - "Quick Select Categories" arranged as a grid of colorful, heavily stylized, outlined illustration chips.
- **Action:** A brightly colored "Save" button with a dark outline.

3. **History List Screen**
- **Header:** "Today's Log".
- **List:** Scrollable list. Each transaction row features the playfully illustrated category icon, ensuring the list feels visually rich and engaging.
- **Bottom Navigation:** A simple bottom bar, but the active state could feature an outlined, illustrative icon rather than a standard thin-line icon.
```
