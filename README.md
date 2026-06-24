# Unique Blue Print — Pharmacy Website (Prototype)

A single-page website for Unique Blue Print, an independent retail pharmacy in South Kolkata, built to extend the pharmacy's day-to-day patient interactions online.

🔗 **Live demo:** https://royakash-cloud.github.io/unique-blue-print-website/

> ⚠️ **Status: Prototype / In Progress.** This is an early build — some buttons and links are placeholders, and the WhatsApp ordering number is not yet connected to the real pharmacy number. Not yet live for actual patient use.

---

## Why this exists

Patients regularly ask for the same kind of help at the pharmacy counter — checking medicine availability, understanding dosage instructions, or knowing when to come back for a follow-up dose. This site is an attempt to extend that counter-side guidance online, rather than build a generic e-commerce storefront.

## Architecture

- Single static HTML file — no backend, no build step, deployed via GitHub Pages.
- WhatsApp deep-linking used for ordering and prescription queries, instead of building a custom order management backend — keeps the pharmacy's existing WhatsApp-based workflow intact while making it easier for patients to start a conversation.
- A `CONFIG` object near the top of `index.html` holds the WhatsApp number, pharmacy name, and location — meant to be updated before going live.

## Planned features

These were chosen based on patterns in the kinds of questions and concerns patients actually raise at the pharmacy counter:

- **Chronic disease lifestyle guidance** — general, educational content (not brand- or dosage-specific, in line with pharmacy advertising norms)
- **Fertility & menstrual cycle awareness tools** for couples
- **Vaccination date calculator** — e.g. automatically calculating Rabies vaccine follow-up dates (Day 0, 3, 7, 14, 28), which are otherwise easy to miscalculate manually

## What's not done yet

- WhatsApp Business number integration (currently a placeholder)
- Linking the planned tools (currently marked "Live" in the UI but not yet wired up)
- Content review for chronic disease guidance to ensure it stays educational, not prescriptive

## Tech

Built with the help of AI-assisted development (Claude Code), as a prototype to validate the concept before deeper investment in functionality.
