---
layout: default
title: Exhibition Portal — User Guide
css: css/style.css
---

# Farnham Urban Sketchers & Friends

## Exhibition Portal — User Guide

A brief walk-through of the whole exhibition lifecycle, in order, showing what each role does and which part of the system they're using. Pairs with `System_Documents_Reference.md` for detail on any specific document mentioned below.

Roles: **Admin** (organiser), **Artist**, **Volunteer** (helps on the day, no login — just a shared PIN).

---

## 1. Setup
**[Admin]** — *Admin Dashboard, Stage 1: Exhibition Setup*
- Set the exhibition name, terms & conditions text, and privacy notice details.
- Set commission rate and payment processing fee rate.
- Set item limits per category, and character limits (title, name, "other" medium).
- Add volunteer names and set the shared PIN volunteers will use for scanning.
- Set label order (title-first or artist-first).
- Set up admin access control (allowed emails + restricted admin URL).
- Confirm Data Mode is set to **Test** for rehearsal, or **Live** once ready for the real exhibition.

## 2. Invite artists
**[Admin]** — *Admin Dashboard, Stage 5: Communications → Invitation*
- Enter recipient emails and send the invitation email, which links to the Entry Portal.

## 3. Submit an entry
**[Artist]** — *Artist Entry Portal*
- Open the link from the invitation email.
- Fill in personal details, artist statement, profile photo, and items across the relevant categories (Hanging, Sculpture, Folios, Sketchbooks, Cards).
- Optionally tick "Show my contact details" and add a website/social media, for the public Artist Info page later.
- Preview before saving, then tick the terms box and submit.
- A confirmation email arrives with a personal link — this is the artist's own return-to-edit link, valid for the rest of the process.

## 4. Edit and monitor entries
**[Artist]** — *Artist Entry Portal (same personal link)*
- Return any time before entries close to add, edit, or remove items.

**[Admin]** — *Admin Dashboard, Stage 2: Monitoring Entries*
- Open the Incomplete Items Report to see who's missing required fields.
- Send reminder emails (Stage 5 → Reminder) — pulled automatically from whoever currently has gaps, with a tickable recipient list.

## 5. Close submissions
**[Admin]** — *Admin Dashboard, Stage 2: Monitoring Entries*
- Toggle "Close Submissions" once ready to finalise.

**[Artist]** — *Artist Entry Portal*
- The form becomes read-only automatically. The artist can still preview, print their profile, and generate labels — just can't edit further.

## 6. Lock numbering and generate documents
**[Admin]** — *Admin Dashboard, Stage 3: Closing & Finalising*
- Lock item numbering (freezes permanent item numbers).
- Optionally enable the Artist Info QR on master labels.
- Generate the Catalogue, Master List, Card Master List, Visual Index, and Artist Profile Sheets as needed.
- Send the closure email (Stage 5 → Closure), letting artists know they can now print their final numbered labels.

**[Artist]** — *Artist Entry Portal (read-only view)*
- Use "Generate My Artwork Labels" to print final labels with real item numbers and QR codes, ready for hand-in.

## 7. Hand-in day
**[Admin / Volunteer]** — *Master List / Card Master List (paper) + Item Status Table / Card Sales Status (screen)*
- Check items in against the printed Master List / Card Master List as artists arrive.
- Mark each item/card batch as Received, either directly on the Item Status Table / Card Sales Status screen, or by scanning the item's own QR code (opens the single-item Update Item Status / Update Card Sale page — first-time scan asks for name + shared PIN).

**[Artist]**
- Brings items with self-printed labels attached (or handwritten numbers if printed before locking).

## 8. During the exhibition
**[Public / Visitors]** — *Artist Info page*
- Scan the QR on an artist's wall label to see their photo, statement, and what else they have on show.

**[Admin / Volunteer]** — *Item Status Table / Card Sales Status, or scan-update pages*
- Record sales as they happen: status, sale price, payment method/reference, buyer signature.
- Card sales are recorded with a simple +/- tap against each batch.
- Concurrent edits are protected — if two people update the same item at once, the second save is flagged as a conflict rather than silently overwriting the first.

## 9. Closing and reconciliation
**[Admin]** — *Admin Dashboard, Stage 4: Exhibition Day & Closeout*
- Mark unsold items as Returned; mark card batches Received/Returned and record physical return counts against the Card Closeout Sheet.
- Check the Item Audit Log / Card Sales Audit Log if any figures look wrong — every change is logged with who, when, and what changed.
- Generate the Sold List and Closing Summary for final financial reconciliation and artist payment.

## 10. Ad-hoc admin edits (any time after locking)
**[Admin]** — *Admin Dashboard, Stage 4 → "Edit Artist Profiles / Add Replacement Items"*
- Look up an artist to edit their profile, add a replacement item after a sale, withdraw an item, or create a new profile for an offline participant. Existing sale/status data is preserved automatically.

---

## Quick reference: who uses what

| Role | Main pages used |
|---|---|
| **Artist** | Entry Portal (edit → read-only), self-print labels, Artist Info page (as a subject) |
| **Admin** | Admin Dashboard (all 5 stages), Item Status Table, Card Sales Status, both Audit Logs, admin edit-entry screen |
| **Volunteer** | Item Status Table / Card Sales Status, or the scanned single-item/card update pages (name + shared PIN, no login) |
| **Public / Visitor** | Artist Info page only |
