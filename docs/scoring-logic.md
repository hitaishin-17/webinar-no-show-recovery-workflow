Replay Engagement Scoring Logic

This document outlines the lead scoring system used in the Webinar Re-Engage Loop to qualify replay viewers and route only high-intent leads to the sales team.

Scoring Triggers  

Trigger Event                Tag Applied                Points              Next Action
Replay Email Opened        opened-replay-email            +5          Wait 24h → Check CTA clicked
Replay Watched 50%+        watched-replay                 +10         Trigger Demo CTA
Clicked “Book Demo” CTA    clicked-demo-link              +20         Create Task for Sales
No Engagement After 48h    cold-no-show                   -10         Move to Nurture Workflow

Engagement Tiers

Score Range                Lead Stage                  Action
25+              SQL (Sales Qualified Lead)      Hand off to Sales team with sql-ready tag
10–24                      Warm Lead             Add to retargeting/remarketing list
<10                        Cold Lead             Enroll into nurture campaign

System Behavior
	•	Only SQLs are routed to Sales.
	•	Task creation includes context (e.g., last action, tags).
	•	Leads below SQL threshold remain in the marketing-owned funnel.
	•	Nurture tracks re-score leads over time based on future activity.
