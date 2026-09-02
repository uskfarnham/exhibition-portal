---
layout: default
title: System Documents Reference
css: css/style.css
---
# Farnham Urban Sketchers & Friends

## Exhibition Portal - System Documents Reference

This lists everything the exhibition portal can produce or display — printable PDFs and live on-screen pages — with what each is for, who uses it, and when.

---

## Printable PDF Documents

| Document | Generated From | Who | When |
|---|---|---|---|
| **My Artwork Labels** | Artist Entry Portal → "Generate My Artwork Labels" | Artist | Any time after saving an entry. Before numbering is locked, labels show title/artist/medium/price only (no number). Once submissions are closed **and** numbering is locked, labels include the item's permanent number and a QR code (links to that item's status-update scan page). 3 copies per item, for self-printing and bringing to hand-in day. |
| **Artwork Labels** (admin master set) | Admin Dashboard → Stage 3 → "Generate Artwork Labels" | Admin | Once submissions are closed and numbering is locked. Master set of labels, one per item, 8 per A4 sheet. Includes an artist-info QR in the corner if that setting is enabled. Backup/reference copy — not usually needed if artists print their own. |
| **Exhibition Catalogue** | Admin Dashboard → Stage 3 → "Generate Exhibition Catalogue" | Admin | Once entries are largely finalised. Full public-facing catalogue, grouped by artist, with statement (if word limit allows) and a table of their items (number, title, size, medium, price). Suitable for printing and handing to visitors. |
| **Master List** | Admin Dashboard → Stage 3 → "Generate Master List" | Admin | Generated once numbering is settled, used through hand-in day and the exhibition run. Ordered by item number (not artist) for fast physical lookup. Working paper checklist: Received / Sold / Sale Price / Signature / Returned columns, filled in by hand. |
| **Card Master List** | Admin Dashboard → Stage 3 → "Generate Cards Master List" | Admin | Hand-in day. One row per card batch — thumbnail, title, artist, price, quantity, a "Received: ☐" box, a QR (once numbering's locked, links to that card's scan/tally page), and ruled tally lines as a paper fallback. |
| **Visual Index** | Admin Dashboard → Stage 3 → "Generate Visual Index" | Admin | Hang-up day. Grid of image tiles (larger than Card Master List's, for actually recognising the artwork), one per item across all four main categories, ordered by item number. Each has a status-update QR. |
| **Artist Profile Sheets** | Admin Dashboard → Stage 3 → "Generate Artist Profile Sheets" | Admin | Once profile photos/statements are in. Wall-display sheets — one (or two) per artist per page, photo + statement. Layout choice depends on the configured statement word limit. |
| **Sold List** | Admin Dashboard → Stage 4 → "Generate Sold List" | Admin | During/after the exhibition, as sales are recorded. Itemised list per artist of everything marked Sold — listed price, sale price, processing fee, commission, amount owed, paid status — with a grand-total footer. |
| **Card Closeout Sheet** | Admin Dashboard → Stage 4 → "Generate Card Closeout Sheet" | Admin | At exhibition close, before physically counting unsold cards. One row per batch: quantity, system-recorded sold count, expected remaining, a blank write-in column for the physically-counted return, and whether it was received at hand-in. |
| **Closing Summary** | Admin Dashboard → Stage 4 → "Generate Closing Summary" | Admin | After the exhibition. One row per artist: items entered, items sold, total sale value, fees, commission, amount owed, paid/unpaid counts. Toggle to include every artist or only those with sales. |

---

## Live On-Screen Pages & Tools

These aren't printed documents, but they're generated/maintained by the system and worth listing alongside the PDFs.

| Page | Who | Purpose |
|---|---|---|
| **Artist Entry Portal** (`Index.html`) | Artist | The main form — submit and edit profile + items. Becomes read-only once submissions close. |
| **Incomplete Items Report** | Admin | Live list of every item/profile missing a required field, with the artist's email, so they can be chased before close. |
| **Item Status Table** | Admin | Working screen for exhibition day — mark items Received/Sold/Returned, record sale price and payment details. Feeds the Sold List and Closing Summary. |
| **Card Sales Status** | Admin | Same idea for card batches — tap +/- to record sales, mark received, record a physical return count. |
| **Item Audit Log** | Admin | Full history of every item-status change (and any blocked/conflicting attempt), with who made it, from where, and when. |
| **Card Sales Audit Log** | Admin | Same for card-tally changes, receipts, and returns — includes a per-card reconciliation summary. |
| **Artist Info Page** (public QR) | Public / visitors | Scanned from an artist's wall label. Shows their photo, statement, and what they have on show, with optional contact details. |
| **Update Item Status** (`scanupdate`) | Volunteers | Scanned from an item's own label/index QR. Lets a volunteer update that single item's status without opening the full admin table. |
| **Update Card Sale** (`cardscan`) | Volunteers | Scanned from a card batch's QR. Single-batch version of Card Sales Status, for quick sale-tally updates on the floor. |
| **Privacy Notice** | Public | Linked from the entry form's consent tickbox. Explains what data is collected and why. |
