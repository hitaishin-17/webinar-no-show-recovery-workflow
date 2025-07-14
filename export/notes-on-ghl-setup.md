
Notes on GHL Setup for Webinar Re-Engage Loop

This document captures important implementation details, considerations, and setup tips within GoHighLevel (GHL) for automating the webinar-to-sales workflow.

⸻

📋 1. Form & Funnel Setup
	•	Registration Page:
Create a funnel with embedded registration form capturing:
	•	Name, Email, Phone Number
	•	Custom field: Timezone (optional but ideal for smart reminders)
	•	Tag on Form Submission:
Apply tag webinar-registered to trigger automation.

⸻

🔁 2. Smart Reminder Workflow
	•	Multi-Channel Sequence includes:
	•	WhatsApp via Twilio integration
	•	SMS & Email Reminders
	•	Voice Drop using GHL Voicemail Drop feature
	•	Use Conditional Waits:
	•	Wait until X time before event
	•	Wait until user responds/clicks
	•	Escalation Flow: if no engagement → switch channel or increase urgency

⸻

🎥 3. Webinar Attendance Tagging
	•	Live attendees: Use Zoom/GHL webhook integration (if available) or manually tag as attended-live
	•	No-shows: After webinar time, auto-tag all non-attendees as no-show

⸻

📽️ 4. Replay & Scoring
	•	Replay delivery workflow:
	•	Triggered by no-show tag
	•	Sends replay link via email and WhatsApp
	•	Tracks engagement using:
	•	Email open → Tag: opened-replay-email
	•	Replay watch (via Wistia/Vimeo hook) → Tag: watched-replay
	•	CTA click → Tag: clicked-demo-link
	•	Add Lead Score using GHL’s Lead Scoring system:
	•	Opened email = +5
	•	Watched replay = +10
	•	Clicked CTA = +20

⸻

🛎️ 5. Notifications & Follow-ups
	•	Sales Task:
	•	Auto-create task for rep if lead score ≥ 25
	•	Notify via Slack/Email integration (optional)
	•	Booking Trigger:
	•	Use GHL calendar link inside CTA
	•	Tag: demo-booked to enter SQL pipeline

⸻

🧰 6. GHL Tips & Best Practices
	•	Use Custom Fields for dynamic tokens in messages (name, time, replay link).
	•	Build Reusable Workflows for tagging, nurturing, scoring — to apply across webinars.
	•	Keep Tag Naming Consistent (e.g., watched-replay, not replay_watched).
	•	Test the flow using a dummy lead with multiple test scenarios (no-show, partial engagement, full engagement).

⸻
