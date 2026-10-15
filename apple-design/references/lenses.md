# Lenses

## Layout and spacing
- Safe areas respected on every edge, including the home indicator and Dynamic Island.
- Consistent spacing scale (4/8/12/16/24/32). Mixed arbitrary values are a finding.
- Alignment: text, icons and controls share a left edge or a centre, never both in one group.
- Readable measure: body text 45 to 75 characters per line. Wider is a finding.
- Nothing floats. Every element belongs to a group with a visible or implied boundary.
- Cards are not a default. Use them only when content is heterogeneous or actionable as a unit.

## Typography
- Use the platform text styles (Large Title, Title, Headline, Body, Callout, Footnote, Caption) or a scale that maps to them.
- Must respond to Dynamic Type or browser font scaling without clipping or overlap.
- At most two typefaces. Weight and size create hierarchy, not colour.
- No orphans in headings. No all-caps body text. Letterspacing only on small caps or labels.

## Colour and contrast
- Text contrast 4.5:1 minimum, 3:1 for large text and icons. Measure it, do not eyeball it.
- One accent colour for interactive elements. If something is the accent colour and not tappable, that is a finding.
- Semantic colours (label, secondaryLabel, systemBackground, separator) over hard-coded hex.
- Colour is never the only signal for state or error.

## Touch and input
- Hit targets 44x44pt minimum, even if the visual is smaller.
- Primary action reachable with the thumb on a phone: bottom third of the screen.
- Destructive actions are red, placed away from the primary action, and confirm when irreversible.
- Correct keyboard type, text content type and autocapitalisation for every field.
- Gestures always have a visible alternative.

## Navigation
- Use the platform's navigation: stack with back button, tab bar for top-level sections, sheets for focused tasks, alerts only for decisions.
- Titles say where you are. Back buttons say where you came from.
- At most five tabs. Hamburger menus are a finding on iOS.
- Modals have a clear way out and never stack more than one deep.

## Motion
- Motion explains a change (where did it come from, where did it go). Motion for delight alone is a finding unless it is a brand moment.
- Durations 200 to 400ms for UI, spring-based on Apple platforms.
- Respect Reduce Motion: crossfade instead of slide, no parallax.
- Nothing loops forever on screen except a progress indicator.

## Accessibility (pass/fail)
- Every control has a label that makes sense read aloud. Icon-only buttons without labels fail.
- Logical reading order. Decorative images hidden from assistive tech.
- Focus visible on keyboard platforms.
- Works at the largest accessibility text size without losing function.
- Announcements for dynamic changes (loading finished, error appeared).

## Copy
- Sentence case for everything except proper nouns. Title Case is a finding on Apple platforms.
- Buttons are verbs: "Save", "Send", "Delete". Never "OK" when a verb fits.
- Errors say what happened and what to do next. Never blame the user.
- No jargon, no exclamation marks, no "please".
