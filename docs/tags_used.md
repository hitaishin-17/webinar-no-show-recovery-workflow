Tags Used — Webinar Re-Engage Loop

This document captures all tags applied throughout the webinar registration, attendance, replay engagement, lead scoring, and sales handoff phases.

⸻

📌 Full Tag List
| **Tag**              | **Purpose / Description**                                   | **When Applied**                                      |
|----------------------|-------------------------------------------------------------|--------------------------------------------------------|
| `attended-live`      | Lead attended the webinar live                              | Right after the live event ends                       |
| `no-show`            | Lead registered but didn’t attend the webinar               | Immediately post-webinar                              |
| `opened-replay-email`| Lead opened the replay email                                | Email open tracked via pixel                          |
| `watched-replay`     | Lead watched at least 50% of the webinar replay             | Triggered by video analytics (or external webhook)    |
| `clicked-demo-link`  | Lead clicked the “Book Demo” CTA in replay email/page       | Link click event from email or page                   |
| `cold-no-show`       | Lead didn’t engage with replay or CTA within 48h            | Triggered after 48h timeout check                     |
| `warm-lead`          | Lead shows moderate intent based on partial interaction     | Score between 10–24 points                            |
| `sql-ready`          | Lead is Sales Qualified and ready for sales engagement      | Score ≥ 25 points or strong CTA click                 |
| `task-created`       | Sales follow-up task created in CRM                         | Triggered post SQL qualification                      |
| `demo-booked`        | Lead successfully booked a demo                             | Tracked via calendar integration or form submit       |

Usage Notes
	•	Tags help drive scoring logic, workflow branching, and CRM segmentation.
	•	Use in tandem with tools like n8n, GHL, or Zapier to trigger actions.
	•	Tag cleanup is recommended monthly to avoid bloat.
