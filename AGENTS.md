# Splash Car Wash: project notes

Read this before making any change to the site.

## The business
- Splash Car Wash, owned by Mr Ehimare Odia, in Okhoro, Benin City, Nigeria.
- Washes cars outside and inside, and also washes at the customer's office or home.
- Open Monday to Saturday, 7am to 8pm. Closed on Sunday.

## The problem this site solves
- Saturday is overcrowded and weekdays are empty. About 150 cars a week, about 60 on Saturdays.
- Office workers want early-morning slots, but many don't know Splash opens at 7am, and they can't wait long because they are rushing to work.
- The site should help customers see the best time to come and move them to quieter days.

## The never rule
- Never promise, confirm or show a guaranteed time slot, especially on Saturdays. Staff confirm every booking.
- Never say a slot is "booked" or "reserved". Use "request" language.
- Staff also confirm every office or home visit.
- Damage complaints go to a person.

## Prices (draft, naira) for sedan/small car | SUV/truck
- Exterior wash: 3,000 | 4,000 (about 30 min)
- Interior + exterior: 5,000 | 7,000 (about 1 hour)
- Engine wash add-on: 3,000 | 4,000 (about 1 hour)
- Office/home service, from: 9,000 | 12,000 (staff confirm time)
- Full auto detailing, from: 20,000 | 30,000 (staff confirm)
- Membership (weekdays only): Basic 10,000 | 13,000 (4 exterior washes), Standard 17,000 | 24,000 (4 interior + exterior), Premium 21,000 | 30,000 (4 interior + exterior and 1 engine wash). One car per membership, one wash per day at most, unused washes expire at month end, staff confirm every visit.

## Design
- Calm, premium, mature and uncluttered. Lots of space, one idea per section.
- Palette: navy #0A1F33 (dark sections), #10304B (deeper panels), aqua #19C3D6 (buttons, badges, accents), white #FFFFFF (text on dark), light panels #F7F9FB with text #1A1A1A (prices, membership, hours, map), muted #9DB6CC (small secondary notes only).
- Alternate dark and light sections. Large, readable text for phones in bright sun.
- One clean sans-serif font. No gradients, no heavy shadows, no crowded cards.
- The hero is a static AI photo. Motion is added later and kept subtle.

## Technical rules
- Static Astro site. No database, no server routes, no logins, no payments.
- No API keys, passwords or tokens in the code. Use a TEST_NUMBER constant for WhatsApp.
- Book a Wash and Join buttons open WhatsApp with a pre-filled message.
- `npm run build` must pass, and the site must deploy on Vercel.
- Mobile first. Images and videos stay small (images under about 300 KB, videos under about 3 MB).
- Respect prefers-reduced-motion.
- Label AI images "AI-generated". Label stock video "Illustrative footage".
- Use real text, never lorem ipsum.
