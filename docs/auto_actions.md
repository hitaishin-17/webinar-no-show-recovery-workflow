Auto-Actions in the Webinar Re-Engage Loop

This document lists all the automation logic applied at various stages of the webinar funnel, from registration to sales qualification.

⸻

🔁 Multi-Channel Reminder Flow
Trigger                                  Action

Registration Submitted              Start smart reminder sequence via WhatsApp, Email, and Voice Drop
No engagement after 1st reminder    Escalate reminder via a second channel (e.g. SMS or WhatsApp)
1 hour before live event            Send AI-powered human-voice drop (“See you there” message)

🎥 Post-Webinar (No-Show Flow)
Trigger                                  Action

No-Show Tag Applied                  Send replay link via email and WhatsApp within 15 minutes
Opened replay email                  Add tag opened-replay-email, add +5 score
Watched 50% of replay                Add tag watched-replay, add +10 score
Clicked “Book Demo” CTA              Add tag clicked-demo-link, add +20 score and create sales task
No activity for 48h                  Add tag cold-no-show, remove 10 points, move to nurture flow

✅ Attendee Flow
Trigger                                  Action

Attended Live                        Add tag attended-live
Attended + Engaged                   Hand off to sales team with sql-ready tag
Booked Demo                          Add tag demo-booked, create calendar invite, notify sales

📬 CRM & Team Notifications
Trigger                                  Action

Lead reaches 25+ score                Notify sales via Slack/Email, create follow-up task
Lead books demo                       Auto-tag as sql-ready, sync to CRM, assign to rep
Sales task created                    Push notification with lead context and CTA

🧠 Smart Scoring System
	•	All engagement actions (opens, clicks, watch time) increase lead score
	•	Cold inactivity decreases score
	•	Thresholds drive automation:
	•	10–24 → Warm lead
	•	25+ → SQL
	•	<10 → Cold/no action → Nurture
