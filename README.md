# webinar-no-show-recovery-workflow

# Grovista Re-Engage Loop (Webinar Replay Automation)

**Built on GoHighLevel (GHL)**  
**Goal:** Rescue webinar no-shows with automated replay workflows and smart lead scoring.

---

## 🔍 Problem

Only 9 out of 50 registrants showed up live.  
But instead of losing the other 41... we turned them into **7 demo bookings** and **2 new customers** – fully automated.

---

## 💡 Solution: The Re-Engage Loop

This project captures and nurtures **no-shows** with:

1. **Multi-channel reminders**  
   Smart WhatsApp + SMS + Email + AI voice nudges, escalated by response tracking.

2. **Instant Replay Distribution**  
   Auto-sent within 15 minutes post-event with a “Book Demo” CTA.

3. **Replay Engagement Scoring**  
   Tag-based scoring to surface high-intent leads.

4. **Lead Routing & Follow-up**  
   leads → sales task created  
   leads → moved to nurture

---
## Product Thinking: Turning No-Shows into Pipeline

This wasn’t just a marketing workflow — it was a product-led initiative driven by real behavior and validated through agile iteration.

**Strategic Thought Process**
- Problem Framing: Only 18% live show-up rate — typical but unacceptable.
- Hypothesis: The replay holds real intent, we’re just not capturing it.
- Goal: Build a system to capture, qualify, and convert that hidden demand.

**Agile Product Flow**
Used Kanban board on JIRA to track:
- Feature ideation
- Experiment cycles
- Funnel optimization tasks
- Weekly review loops to improve engagement timing, tag rules, and CTA wording.


**Data-Driven Design**
Created lead engagement scorecards based on:
- Replay open time
- Tag triggers (e.g., watched_75, clicked_cta)
- Channel response (Email/SMS/WhatsApp/AI Voice)
- Mapped conversion journey from replay → to booking → to follow-up

**Learnings Logged**
- Tags > Clicks — Intent hides in behavior, not just actions
- Follow-up timing ≠ event end → it’s ~2 hours after replay delivered
- GHL limitations suggest next version may be external microservice


```
📂 grovista-reengage-loop/
├── README.md                         # Project overview and purpose
├── loom-demo.md                      # Loom link and video walkthrough
├── funnel-overview.png               # Visual of the full funnel journey

├── assets/
│   ├── reminders-flow.png            # Diagram of multi-channel reminders
│   ├── replay-engagement-tags.png    # Replay scoring flow
│   └── engagement-tags-detailed.png  # Visual: tag + trigger + next step logic

├── docs/
│   ├── workflow-summary.md           # Step-by-step breakdown of the entire flow
│   ├── scoring-logic.md              # Lead scoring points, tags, thresholds
│   ├── tags-used.md                  # Table of all tags, purpose, and when applied
│   └── auto-actions.md               # Auto-triggers for reminders, tasks, and handoffs

├── export/
│   └── notes-on-ghl-setup.md         # Implementation notes since GHL doesn’t export flows
```

## 🎥 Demo

→ [Check out the video walkthrough](https://drive.google.com/file/d/1RMxwakXs3-317tyzagsjKOrS_YumC_m8/view?usp=sharing)

## Results

- **41 no-shows**  
→ 23 replay views  
→ 7 demo bookings  
→ 2 new customers  
→ All on autopilot 🎯

---

## Built With

- GoHighLevel (GHL)
- Webhooks + Tag Automation
- Custom Scoring
- Smart follow-up logic

---

## Learnings

- The real pipeline often hides in the replay.
- Engagement tags > Just open tracking.
- Timing and channel mix matter.

---

## Questions?

[Connect with me on LinkedIn](www.linkedin.com/in/hitaishi-n-grovista)

---
