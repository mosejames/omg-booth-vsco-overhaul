# VSCO Workspace - Automations

Automations consist of three components: Observables (Triggers), Conditions, and Actions.

## Observables (Triggers)

The event or occurrence the automation looks for to trigger it.

### Known Observables:
- **Lead > Created** -- When a new lead is created
- **Lead > Lead Status Changed** -- When a lead status changes (runs immediately or at 8am studio time)
- **Calendar > Meeting** -- Based on meetings on the calendar
- **Calendar > Session** -- Based on sessions on the calendar
- **Calendar > Call** -- Based on calls on the calendar
- **Task > Completed** -- When a task is checked off
- **Bookable Event scheduling** -- Related to online scheduling events

### Execution Timing:
- **Immediately** -- Runs as soon as the observable fires
- **Relative to an event** -- E.g., "3 days before" a meeting. System checks for scheduled events and executes if today matches the relative timing
- **At 8am studio time** -- On the day specified in the Execute box

---

## Conditions

Conditions narrow down when the automation should run.

### Known Conditions:
- **Job Stage Condition** -- Only run if job is in a specific stage (Lead, Booked, Fulfillment, Completed)
- **Job Type Condition** -- E.g., "if the job type contains Maternity or Newborn"
- **Web Lead Condition** -- "If the new lead is a web lead (wasn't created manually)"
- **Scheduling Condition** -- Prevents automations from running when a client schedules a Bookable Event

---

## Actions

What the automation performs.

### Available Actions:
1. **Send Email** -- Sends an email using a template; tracking shows Sent, Delivered, Opened, Read, Link Clicked
2. **Add Task** -- Creates a new task (configurable: task list name, task name, due date, assignee)
3. **Add Event** -- Adds a calendar event
4. **Update Field** -- Updates any field in the database using tokens
5. **Post Web Request** -- Sends a webhook to external services (useful for Zapier)

---

## Template Gallery

Browse and install pre-built automations from industry professionals:
- Auto-respond to new leads
- Out-of-office auto response
- Meeting/session reminders
- Follow-up reminders
- Task completion chain triggers

---

## Common Automation Examples

### Auto-Respond to New Leads
- **Observes:** Lead > Created
- **Executes:** Immediately
- **Condition:** Web Lead (wasn't manually created)
- **Action:** Send auto-response email
- Can filter by job type (e.g., only for Maternity or Newborn inquiries)

### Meeting/Session Reminder
- **Observes:** Calendar > Meeting
- **Executes:** 3 days before (or custom)
- **Action:** Send reminder email
- Use `{{target.channel_details}}` token for meeting location/link

### Lead Follow-Up
- Set a rule on "Initial Contact" lead status to automatically change to "Needs Follow Up" after X days
- **Observes:** Lead > Lead Status Changed
- **Condition:** Status is "Needs Follow Up"
- **Action:** Send follow-up email and/or add task

### Task Chain
- **Observes:** Task > Completed (e.g., "Follow up on image selection")
- **Action:** Create another task due in 5 days + send email to client

### Auto-Send Quote to New Lead
- **Observes:** Lead > Created
- **Executes:** Immediately
- **Action:** Send email with quote link

---

## Execution History

- Shows if an automation failed or triggered successfully
- Provides reasons why an execution was skipped
- Useful for debugging automation issues

---

## Scheduling Conditions

- Prevents automations from running when a client schedules a Bookable Event
- Can be reviewed and applied automatically via the Review button in the banner
- Or manually added to individual automations
- Accessible at workspace.vsco.co/settings/automations/scheduling-conditions
