# wheredidtimego
A browser-based time tracker for logging how you spend your time across different categories.

**Development note:** This project was developed using AI-assisted coding (often referred to as "vibe coding"). I designed the features and iterated on the application, using AI tools to help generate and modify the code.

## Version History

### V1: Core Time Tracking

* **Category timers:** Start, pause, resume, and finish a timer for each category.
* **Today and history:** View today's time by category and browse full history by day, with expandable daily records.
* **Manual editing:** Add or edit sessions to correct forgotten starts or stops, including sessions containing multiple intervals.
* **Custom categories:** Create your own categories and assign them a colour.
* **CSV export:** Export today's data or your complete history as CSV, with one row per interval containing the date, category, start time, end time, and duration.
* **Local storage:** Data is stored in the browser's localStorage, allowing it to persist between visits on the same device and browser.

### V2: Categories and Context

* **Session descriptions:** Add an optional description when starting a timer. Descriptions are also included in CSV exports.
* **Category emojis:** Assign an emoji to each category. New categories can be given an emoji alongside their colour.
* **Default categories:** Added Exercise 🏃, Socialising 🗣️, Art 🎨, Time-wasting 🕳️, and Sleep 😴 alongside Studying 📚, Reading 📖, and Admin 🗂️.

### V3: Goals and Visualisation

* **Category targets:** Set an optional daily target in minutes for each category.
* **Progress chart:** Select a category and date range to compare cumulative time logged against a target pace line.
* **Timeline:** A Gantt-style timeline shows when sessions occurred during each day, making it easier to identify patterns in when time is spent.
* **Adjustable timeline:** Choose the time window displayed, with a default of 14 days.

### V4: Organisation and Interface

* **Tabbed navigation:** Organised the app into three tabs:

  * **Timer:** Active timer, Today, and History
  * **Graphs:** Progress and Timeline
  * **Categories:** Category management and Export
* **Category colours:** Updated the colour scheme for each default category.
* **Layout improvements:** Fixed category row alignment.

### V5: Data Management and Insights

* **CSV import:** Import previous exports and merge them with existing data. Categories are matched by name, new categories are created automatically, and duplicate rows are skipped when the same file is imported again.
* **Export reminders:** A banner appears after three days without an export, with a one-tap **Export all** button.
* **Category archiving:** Categories can now be archived instead of immediately deleted. Archived categories are moved to a collapsed list where they can be restored or permanently deleted. Existing sessions retain their original category name, colour, and emoji.
* **By-weekday chart:** Added a bar chart showing total time per weekday from Monday to Sunday for the selected category and date range.
