# OMG Booth — VSCO Workspace Questionnaire Cleanup

**Date:** February 10, 2026  
**Project:** Restructuring client intake questionnaires in VSCO Workspace (formerly Táve Studio Manager)

---

## Company Overview

**OMG Booth** is an Atlanta-based experiential media company that helps brands, schools, and organizations capture attention and turn moments into shareable content.

### Services
- **Photo Booth Experiences** — Professional lighting, custom overlays, instant delivery via text/email. Digital-first, prints available.
- **Social and Content Booths** — GIFs, Boomerangs, short videos designed for social sharing.
- **On-Site Activations** — Branded experiences for conferences, campuses, corporate events, sporting events, community programs. Full setup, staffing, and guest flow management.
- **Custom Branding and Design** — Event-specific frames, overlays, step-and-repeats, visual systems matched to client brand.
- **Data and Follow-Up Assets** — Opt-in lead capture, curated galleries, post-event content for reuse.

### Clients
- Brands and agencies
- Schools and universities
- Corporate teams and employee groups
- Nonprofits and community organizations
- Private events wanting a polished, professional experience

### Differentiators
- Experience-first approach, not just equipment
- Clean, intentional, modern setups
- Fast content delivery to guests
- Reusable assets for clients beyond the event
- Calm, professional on-site presence

---

## CRM Platform

**VSCO Workspace** (formerly Táve Studio Manager, acquired by VSCO in May 2025, launched August 2025). Features include questionnaire builder with basic/advanced/layout fields, visibility controls, automation workflows, client portals, contracts, and invoicing.

---

## Current State: 26 Existing Questionnaires

### Full Inventory

| Questionnaire | Responses | Status |
|---|---|---|
| Contact Form Inquiry Step 2 - Additional Info | 0 | Dead — candidate for deletion |
| Design Assets Review | 1 | Near-dead |
| Event Customizations - 360º | 3 | Low use |
| Event Customizations - Design + Props | 5 | Low use |
| Event Customizations - Design + Props + Social | 18 | Moderate use |
| Event Customizations - Design + Props + Social + Microsite | 53 | Active |
| Event Customizations - Design + Social | 30 | Active |
| Event Customizations - Design + Social + Microsite | 2 | Near-dead |
| Event Customizations - Desing + Social (Bragbox) | 0 | Dead — typo in name |
| Event Customizations - First Day of School | 1 | Near-dead |
| Event Customizations - Props Only | 2 | Near-dead |
| Event Customizations - Virtual Booth | 28 | Active |
| Event Customizations - Virtual Booth Info | 45 | Active |
| Event Logistics | 402 | **Workhorse** |
| Logistics - Corporate Event | 0 | Dead |
| Logistics - Holiday Event | 6 | Low use |
| Logistics - Social Event | 59 | Active |
| Logistics - Wedding | 21 | Active |
| New Lead In-take | 0 | Dead |
| New Lead Logistics - Virtual Booth | 181 | **Heavy use** |
| Photo Booth Intake Questionnaire | 1 | Near-dead |
| Reports - Post-Event Report [Experience Manager] | 139 | **Heavy use** |
| Reports - Post-Event Report [Smile Squad] | 65 | Active |
| Reports - Pre-Event Report | 101 | **Heavy use** |
| Step 2 of 2 — Event details | 84 | Active |
| Virtual Booth Event Logistics | 47 | Active |

### Key Problems
1. **11 "Event Customizations" variants** — each built for a specific service combo. Doesn't scale when packages change.
2. **4 separate Logistics forms** — Corporate, Holiday, Social, Wedding plus the main Event Logistics.
3. **Multiple dead/near-dead forms** with 0-2 responses cluttering the workspace.
4. **No single clean intake path** — leads hit different forms depending on service type.

---

## Proposed Consolidation: 26 → 6 Forms

### 1. New Lead Intake (Public-Facing)
First touchpoint for all new leads. Short, fast qualification.
- Event type
- Date
- Estimated guest count
- Organization name
- Referral source
- Desired experience type (photo booth, GIF/video, branded activation)

### 2. Event Details (Post-Interest)
Sent after initial conversation, before proposal. Replaces all 11 "Event Customizations" variants using conditional logic or smart sections.
- Venue name and address
- Indoor/outdoor setup
- Power access
- Load-in logistics
- Branding requirements
- Print vs. digital-only preference
- Lead capture needs
- Content goals

### 3. Event Logistics (Post-Booking)
Merges 4 logistics variants into one unified form.
- Venue/setup details
- Day-of contact info
- Setup window
- WiFi info
- Special requests

### 4. Design & Branding Brief
One form for collecting all creative assets and preferences.
- Logos, colors, fonts
- Overlay/frame design preferences
- Approval workflow

### 5. Pre-Event Report (Keep Existing)
Already working well with 101 responses. Review for any needed updates.

### 6. Post-Event Report (Merge)
Combine Experience Manager (139 responses) and Smile Squad (65 responses) versions into one form with a role selector.

---

## Next Steps

1. **Review all 26 existing questionnaires** to see actual field content — identify what to keep, merge, and cut
2. **Determine VSCO Workspace conditional logic capabilities** — can fields show/hide based on answers, or do sections need to be visible and labeled?
3. **Draft consolidated questionnaires** question by question
4. **Build in VSCO Workspace** and test

### Recommended Approach for Review
- Open each questionnaire in VSCO Workspace via browser
- Claude can navigate through them directly using Chrome browser tools if Workspace is open
- This captures actual field types, required vs. optional settings, and any existing conditional logic

---

## Handoff Notes for Claude Cowork

This project is moving to Claude Cowork for the hands-on browser work of reviewing all 26 forms and building the consolidated replacements. Key context:

- **Workspace URL:** https://workspace.vsco.co/forms/all
- **Goal:** Review all 26 forms via browser, then build 6 consolidated replacements
- **Company:** OMG Booth (Atlanta experiential media — photo/video booths, branded activations)
- **CRM:** VSCO Workspace (formerly Táve Studio Manager)
