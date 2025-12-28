<!-- CANONICAL: lifecycle -->

---
title: "Page Lifecycle"
slug: "lifecycle"
---

# Page Lifecycle

This document defines the only allowed lifecycle states for content pages.

## Status values (allowed)

All factual pages MUST include a frontmatter field:

- `status: draft | pending-review | verified | archived`

No other values are permitted.

## What each status means

### `draft`
Work in progress.
- Not presented as fact.
- May be incomplete, unreviewed, or missing sources.

### `pending-review`
Ready for review.
- Claim is fully stated.
- Sources are attached and formatted.
- Waiting for reviewer approval.

### `verified`
Approved for publication as factual record.
- Reviewer has approved.
- Every factual statement has a clickable source.
- Any uncertainty is explicitly labeled as disputed/uncertain.

### `archived`
No longer actively maintained.
- Kept for record.
- Must remain readable and referenced, but not treated as current.

## Publishing rule (non-negotiable)

Only pages with:

- `status: verified`

may be treated as authoritative factual pages.

All other statuses MUST be treated as non-authoritative.

## Required fields for factual pages

Factual pages MUST include these frontmatter keys:

- `status`
- `created`
- `updated`
- `review_required: true`
- `reviewer: PAA-Reviewer`
