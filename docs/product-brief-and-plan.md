# One-page product brief

## One-line scope

Help a student paste a class announcement, review its extracted details, save a deadline, and track it to completion in one simple web app.

## Problem and target user

Students receive assignments, quizzes, lab updates, registration notices, and study links across class groups. Important dates and materials are easy to lose in the conversation. The target user is a student who needs one place to organize those updates without a complicated setup.

## Core user journey

Open the dashboard → paste an announcement in Message capture → extract suggested details → review or correct the date, time and link → save the deadline → find it in the list or calendar → mark it complete. Save useful study links as resources when appropriate.

## Must-have scope used for this submission

1. Dashboard with workload counts.
2. Add, edit, delete and complete deadlines.
3. Calendar view.
4. Capture pasted messages with editable suggestions.
5. Saved resource links and notes.
6. Persist data in the current browser and provide a usable phone layout.

## Technology and data choice

HTML defines the screens and forms; CSS provides the layout and responsive rules; JavaScript manages tasks, parsing and views. localStorage saves data in the current browser. GitHub stores the source, and ChatGPT Sites hosts the public app. No backend, account system, database service or paid AI API is required for this local-data scope.

## Reference wireframe

| Screen | Layout and primary action |
| --- | --- |
| Dashboard | Navigation + search; workload summary cards; upcoming deadlines; saved resources; Add deadline. |
| Message capture | Pasted message box; Extract details; suggested details; Save as deadline / Save as resource. |
| Deadline form | Title, category, subject, due date/time, priority, source, URL and notes; Save deadline. |

This is a text wireframe reflecting the existing interface; the supplied demo provides actual screen references. The scope above is reconstructed from the requested functionality, rather than a separately supplied original Must-have list.

## Success criterion and exclusions

A first-time user can save one deadline from a pasted message and mark it complete without help. Automatic WhatsApp access, cloud sync, collaboration, and alerts while the page is closed are outside this MVP.

# Agent implementation plan and file guide

Plan status: This implementation plan is prepared now to explain and reproduce the existing MVP. It is not presented as evidence that a plan was approved before coding.

| Step | Implementation task | Acceptance check |
| --- | --- | --- |
| 1. Structure | Create dashboard, deadline list, calendar, capture, resources and settings views. | Navigation opens the intended view. |
| 2. Data | Define task and resource objects; load/save JSON in localStorage. | Save a task, refresh, and confirm it remains. |
| 3. Deadlines | Add forms, validation, editing, deletion and completion. | Create a task, edit it, complete it, then delete a disposable task. |
| 4. Capture | Extract a link, supported date/time and category using JavaScript patterns. | Paste a known example; review suggestions and save it. |
| 5. Views | Render counts, date order, filters, calendar and resources. | Saved task appears in the list and correct calendar day. |
| 6. Finish | Use responsive CSS, export/import backup and input checks. | Check a phone screen and round-trip a test backup. |
| 7. Deliver | Commit source, publish, record the core task. | Live link opens and a new user completes the journey. |

## What each file or code section does

| File / section | Plain-language explanation |
| --- | --- |
| index.html: HTML | Defines the buttons, cards, navigation, forms and screen sections. |
| index.html: CSS | Controls colors, spacing and layout, with breakpoints for smaller screens. |
| index.html: JavaScript | Stores the data model and reacts to clicks; updates the interface after changes. |
| parseMessage() | Uses text patterns to suggest a date, time, category and URL. It is rule-based extraction, not an AI model. |
| saveForm(), save() | Validate form entries, update tasks/resources and write browser storage. |
| render(), renderCalendar() | Rebuild the dashboard, lists, progress summaries and month grid from saved data. |
| README.md | Explains the features, local use, live URL and hosting limitations. |
