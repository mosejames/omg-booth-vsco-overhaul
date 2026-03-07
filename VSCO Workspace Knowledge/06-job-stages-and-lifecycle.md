# VSCO Workspace - Job Stages and Lifecycle

## Four Job Stages

### 1. Lead
The initial stage when a potential client first contacts you.

**How leads are created:**
- Manually via the New Lead option on the dashboard
- Automatically through a VSCO Workspace contact form on your website
- Automatically through a public questionnaire (if set to auto-create lead)
- Via Zapier integrations (e.g., Acuity Scheduling, Calendly)

### 2. Booked
When a client agrees to work with you, the lead becomes a "job."

**Automatic transition:** A lead automatically moves to Booked when:
- A client signs a contract
- A client agrees to/approves a quote

The approved quote becomes an order.

### 3. Fulfillment
The working stage -- after booking, during service delivery.

### 4. Completed
The final stage of a successfully fulfilled job. Move here after completing all tasks.

---

## Completed vs. Closed

This distinction is critical for accurate reporting.

### Completed
- Used when a job has been properly fulfilled through all stages
- The natural end of a successful job lifecycle
- Properly tracked in booking reports and conversion rates

### Closed
- Used ONLY when:
  - A new lead does not end up booking
  - A booked job cancels
- When closed, all upcoming events are canceled and outstanding invoices are voided
- You must select a close reason (why they're not booking/continuing)
- For canceled jobs, payments already made remain intact

**WARNING:** If you close jobs that were actually completed, it causes inaccuracies in:
- Job conversion rates in booking reports
- Lead closed reason reports
- Revenue and financial reporting

---

## Closing a Lost Lead or Canceled Job

1. Click the Close button on the job's overview screen
2. Select a close reason
3. For canceled jobs: remaining open orders are voided, but payments made stay intact
4. You can bulk-close multiple leads at once with the same closed reason

---

## Deleting a Lead or Job (Purge)

To permanently delete a lead/job:
1. First Close the lead/job (select a close reason)
2. Then Purge it -- this permanently removes it as if it never existed
3. Cannot be undone

---

## Job Stage Condition in Automations

You can add a Job Stage condition to automations so they only run when a job is in a specific stage (Lead, Booked, Fulfillment, or Completed). This prevents automations from firing at the wrong time.
