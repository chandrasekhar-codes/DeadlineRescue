# Feature checklist: status and reasons

Status key: Done = implemented in the inspected source; Partial = works within a stated limitation or still needs user validation; Cut = intentionally excluded. Source review and the supplied recording do not replace a full device test.

| Feature | Status | Reason / evidence |
| --- | --- | --- |
| Student dashboard | Done | Counts active, due-soon, completed tasks and resources; visible in the demo. |
| Deadline task management | Done | Forms and handlers support create, edit, delete and completion; demo shows saving and marking complete. |
| Calendar | Done | Month navigation and deadline date cells are implemented; visible in the demo. |
| Pasted message capture | Done | Paste, extract, review and save actions are implemented. User confirmation is required before saving. |
| Automatic date understanding | Partial | Recognizes supported patterns only. Ambiguous or missing dates need manual correction. |
| Saved resources | Done | Resource forms, notes, optional URLs, opening, editing and deletion are implemented; resource view is shown in the demo. |
| Data persistence | Done | localStorage retains data in the same browser; export/import provides manual backup. No cloud sync. |
| Responsive phone layout | Partial | Responsive CSS and a mobile navigation toggle exist. Real phone usability has not been recorded. |
| Progress insights | Done | Existing completion and category summaries are retained; visible in the demo. Supporting feature beyond the core journey. |
| Backup export/import | Done | JSON download, import checks and restore handlers exist. Manual round-trip testing has not been recorded. |
| Browser notifications | Partial | Requires browser permission and the page to remain open. Closed-page alerts are excluded. |
| Public deployment | Done | Sites reports active status with public access. Hosting provider acceptance depends on course rules. |
| Automatic WhatsApp access | Cut | The MVP accepts pasted messages only; no account connection or chat scanning. |
| Accounts, cloud sync, collaboration | Cut | Excluded to keep the browser-local MVP small. |
| Automatic GitHub deployment | Cut | Repository stores source; updates to the live Site require separate publication. |

No feature changes were made solely for this assignment pack. Existing progress and backup tools are documented as supporting features; no new scope was added.
