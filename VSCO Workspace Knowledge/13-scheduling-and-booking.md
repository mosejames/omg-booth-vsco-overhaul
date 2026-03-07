# VSCO Workspace - Scheduling and Booking

## Bookable Events

**Location:** Scheduling sidebar > Bookable Events

A Bookable Event is a scheduler you set up with certain availability for clients to book a meeting, call, session, or mini session.

### Creating a Bookable Event:
- **Event Type** (e.g., Discovery Call, Pre-Wedding Meeting, Headshot Session)
- **Event Name**
- **Booking Site** assignment
- **URL** for the event
- **Lead Type** -- what type of lead this creates
- **Event Description** and **Event Header**
- **Public or Private** setting

### Availability:
- Set your available hours for each event type
- Events check your Workspace calendar and connected calendars for conflicts
- Clients can schedule and book completely unassisted based on real-time availability

---

## Public vs. Private Bookable Events

### Public Events:
- Visible on your public booking site when visited without a private invitation
- Anyone can see and book

### Private Events:
- NOT listed on your booking site
- Available only at the bookable event's direct URL
- Must be shared individually

### Sending Invitations:
- Send invitations to either type from any lead or job's Schedule tab
- Use the "New Invitation" dropdown

---

## Booking Sites

- Public events are organized under Booking Sites
- Only admin/billing users can manage Bookable Events, Mini Sessions, Availability, and Booking Sites (Standard users don't have access)

---

## Mini Sessions

Mini Sessions allow clients to book from specific dates and time slots (unlike regular bookable events which use availability schedules).

### Creating Mini Sessions:
1. Navigate to Scheduling sidebar > New Bookable Event for Mini Sessions
2. Configure event type, name, booking site, URL, job type
3. Add description and header
4. Set as public or private

### Dates, Times, and Locations:
- Select specific dates in the calendar
- Can select multiple dates for the same location
- Enter location to see weather, sunrise, and sunset times
- NO Availability section -- you set exact dates, times, and locations

### Key Differences from Regular Bookable Events:
- Do NOT use an availability schedule
- Do NOT check Workspace calendar or connected calendars for conflicts
- Dates and time slots are offered regardless of other calendar events

### Confirmation and Reminders:
- Customize confirmation email sent when a Mini Session is booked
- Add event reminder notice emails (e.g., 1 hour before, 24 hours before)
- Can set up multiple reminders

### Manually Holding Time Slots:
- Use the Hold button next to a slot to prevent online booking
- Hold for a specific client or to appear busy
- Remove holds at any time
- When a client books from an invitation, it's added to their existing lead/job

---

## Embedding Bookable Events

1. Go to Scheduling > Bookable Events
2. Use the Actions dropdown > Embeddable Link
3. Opens in new tab showing the inline URL (contains `-inline`)
4. Use iframe code with the inline URL:

```html
<iframe id="bookable-event" src="[your-inline-url]" width="100%" height="1100px" frameborder="0" scrolling="no"></iframe>
```

Requires access to your webpage's HTML source code.

---

## Text Notifications for Bookable Events

Set up automatic text message notifications:
- Stale booking reminders
- Confirmation notices
- Reminder notices to event attendees

Select "add text notification" option on the bookable event configuration.
