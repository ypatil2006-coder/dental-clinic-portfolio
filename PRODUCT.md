# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

delegated: static HTML/CSS/JS (no build step; fastest path to a reviewable mobile-first one-pager in this workspace)

## Users

Primary: prospective patients in the clinic's local area, arriving on a phone, deciding whether to trust one specific dentist and take the next step. Their job is to judge competence and warmth quickly, then make contact.

Secondary: the dentist themselves, who wants a personal, portfolio-style presence rather than a generic clinic brochure.

## Product Purpose

A single-page web presence for a dental practice run by one person. Its job is to present that person and their work with the credibility of a professional portfolio, and convert visitors into WhatsApp enquiries.

Success: a visitor understands who the dentist is, what they do, and taps the WhatsApp CTA with a pre-filled message.

## Positioning

Unlike a multi-dentist clinic site that sells a facility, this site puts one practitioner forward as the subject — their story, their work, their standard of care — using the visual language of a personal design portfolio.

## Operating Context

- Mobile-first; the phone viewport is the primary design target.
- Appointment booking happens only through WhatsApp, using a `wa.me` deep link with a pre-filled message.
- No booking form, no payment, no patient portal.
- Content not supplied by the client is placeholder and must be labelled as such.

## Capabilities and Constraints

- One scroll-driven page.
- One primary action: WhatsApp appointment button, repeated at the close.
- Sections: hero, selected work / smile gallery, about the dentist, approach, one patient testimonial, contact.
- Dentist name, WhatsApp number, clinic location, and credentials are unresolved; use placeholders.
- No invented testimonials, qualifications, prices, or results presented as real.

## Brand Commitments

- The client explicitly chose a clean, mobile-first, minimalist, premium aesthetic.
- The client explicitly asked to mimic melon.studio: portfolio-style, one-person voice, dark/red editorial motion language, strong typography, scroll and hover animation.
- The site is run by a single person, so the voice is first-person singular.

## Evidence on Hand

- Reference captures from melon.studio: `/tmp/opencode/melon/scroll.mp4`, `/tmp/opencode/melon/contact.jpg`, `/tmp/opencode/melon-hover/pairs.jpg`.
- No real clinic photography, name, number, credentials, or testimonials supplied. All such content is authored as labelled placeholder.

## Product Principles

1. The person is the product — lead with the practitioner, not the clinic.
2. One action only — every path ends at the WhatsApp CTA.
3. Restraint over feature count — a few excellent sections, not many mediocre ones.
4. Motion is material, not decoration — motion should clarify sequence and focus.
5. Nothing fabricated — placeholders are visible and replaceable.

## Accessibility & Inclusion

Inferred, not confirmed: respect `prefers-reduced-motion`, maintain legible contrast, keep all content reachable without hover, and keep tap targets comfortably sized on mobile.
