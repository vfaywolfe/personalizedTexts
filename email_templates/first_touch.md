# Template: First Touch — Educator variant (marketing/templates/first-touch.md)

## Merge fields
| Field | Source |
|---|---|
| {{firstname}} {{lastname}} | firstname, lastname |
| {{jobtitle}} | jobtitle — convention: includes department ("Associate Professor, Computer Science") |
| {{institution}} | associated company name |
| {{discipline}} | derived from the department in jobtitle |
| {{course}}, {{current_materials}}, {{hook}} | OPTIONAL — usually unknown at first touch |
| {{segment}} | author_segment |
| {{sender_name}} | the intern composing (from prompt context, not HubSpot) |

## Personalization tiers
- Tier 1 — we found something specific (a course, materials, a talk, a post): open with it;
  every claim about the recipient traces to the notes.
- Tier 2 — name + department only (the common case): open with honest department-level
  relevance. NEVER imply we know what they teach; no fake hooks, no "loved your work."
- 60-second upgrade rule: before drafting, check the department's faculty/course page for
  {{lastname}} — one found course upgrades Tier 2 → Tier 1 and gets noted on the contact.

## Composition rules
1. ≤ 175 words. Subject ≤ 8 words, no clickbait, no "quick question." The easy-authoring /
   professional-product contrast is the core pitch — never present ease without immediately
   anchoring the polish and faculty-grade features of the result.
2. Tier 2 uses {{discipline}}, never {{course}} or any specific we don't have.
3. ONE primary CTA; Tier 2 defaults to LOW or MEDIUM — a cold recipient hasn't earned a
   meeting ask.
4. Revenue angle: ONLY for OER Author / Independent Instructor segments (→ use B.1-C instead).
5. Discipline-flavor the value prop: CS/STEM → autograded coding; other disciplines →
   interactive activities + AI tutor. Sample-book link only if one matches {{discipline}}.
6. Plain text, ≤ 2 links, warm colleague tone, real-name signature. Never promise features
   or dates. Pricing: exactly two approved statements — "authoring is always free" and
   "student cost is a small fraction of a typical textbook" — never specific numbers.

## CTA ladder
- LOW → the 2-minute vision video at https://www.curacourse.com/
- MEDIUM (Tier 2 default) → free account + first lesson: "live in under 30 minutes"
  (https://www.curacourse.com/signup)
- HIGH (Tier 1 with strong hook only) → 20-minute walkthrough with the founding team

## Body — Tier 2 (name + department only)

Subject "CuraCourse Teach Your Way - Author Your Own Textbook Quickly and Easily"
Hi Professor {{lastname}},

I'm writing to {{discipline}} faculty at {{institution}} because most of us teach from a textbook that almost works — a chapter that doesn't fit the syllabus, examples that feel dated, no way to just edit the thing.

CuraCourse fixes that. Adapt your proven curriculum and make the textbook yours, or build your own. You don't have to start from a blank page: hand the CuraAI authoring assistant the materials you already teach with (slides, articles, handouts, lecture notes) and it blends them into your book. The result is a polished, professional textbook: high-quality interactive exercises {{discipline-flavored — CS/STEM: "with autograded coding in Python, Java, C++ and more, using test cases you control"}}, automatic grading, and an AI tutor that coaches students with Socratic questions - even when they're stuck at 11pm. You get a live dashboard of every student's work, like who's practicing and who's stuck, before the exam tells you. Grades sync to your LMS. Authoring is always free, and the student cost is a small fraction of a typical textbook. Join faculty at institutions across the country who are creating their own textbook quickly and easily.

{{ONE CTA — e.g., "If you're curious, a free account takes a minute and a first interactive lesson about 30: https://www.curacourse.com/signup"}}

Best,
{{sender_name}}
CuraCourse — https://www.curacourse.com/
