
Notes on GHL Setup for Webinar Re-Engage Loop

# 📓 Notes on GHL Setup for Webinar Automation Workflow

This document captures important implementation details, considerations, and setup tips within GoHighLevel (GHL) for automating the webinar-to-sales workflow.

---

## 📋 1. Form & Funnel Setup

- **Registration Page**:  
  Create a funnel with an embedded registration form capturing:
  - Name, Email, Phone Number  
  - Custom Field: `Timezone` *(optional but ideal for smart reminders)*

- **Tag on Form Submission**:  
  Apply tag `webinar-registered` to trigger the automation sequence.

---

## 🔁 2. Smart Reminder Workflow

- **Multi-Channel Sequence Includes**:
  - WhatsApp via Twilio integration  
  - SMS & Email Reminders  
  - Voice Drop using GHL Voicemail Drop feature  

- **Use Conditional Waits**:
  - Wait until X time before event  
  - Wait until user responds or clicks  

- **Escalation Flow**:  
  If no engagement → switch channel or increase urgency (e.g., voice drop or direct SMS)

---

## 🎥 3. Webinar Attendance Tagging

- **Live Attendees**:  
  Use Zoom ↔ GHL webhook integration (if available) or tag manually as `attended-live`.

- **No-Shows**:  
  After webinar time, auto-tag all non-attendees with `no-show`.

---

## 📽️ 4. Replay & Lead Scoring

- **Replay Delivery Workflow**:  
  Triggered by `no-show` tag — sends replay link via:
  - Email  
  - WhatsApp  

- **Engagement Tracking Tags**:
  - Opened replay email → `opened-replay-email` (+5 points)  
  - Watched 50%+ of replay (via Wistia/Vimeo webhook) → `watched-replay` (+10 points)  
  - Clicked “Book Demo” CTA → `clicked-demo-link` (+20 points)

- **Lead Scoring**:  
  Use GHL’s native Lead Scoring system to assign points automatically.

---

## 🛎️ 5. Notifications & Follow-ups

- **Sales Task Creation**:
  - If lead score ≥ 25 → auto-create task for sales rep  
  - Optional: Notify via Slack or Email integration  

- **Booking Trigger**:
  - Embed GHL calendar link in CTA  
  - Tag `demo-booked` when a booking is made  
  - Trigger `sql-ready` workflow and sales handoff

---

## 🧰 6. GHL Tips & Best Practices

- Use **Custom Fields** to personalize messages (e.g., first name, event time, replay link)
- Create **Reusable Workflows** for tagging, nurturing, and scoring — to standardize across all webinars
- Maintain **Tag Naming Consistency**  
  *(e.g., use `watched-replay` instead of `replay_watched`)*  
- **Test Extensively**:  
  Use dummy leads to simulate:
  - No-show  
  - Partial engagement  
  - Full engagement  
  - Demo booked

---

