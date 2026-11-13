# aidevfest.org

Event site for **DevFest Phoenix × sunhacks ASU 2026** (Saturday, November 14, 2026, 9 AM to 6:20 PM, Student
Pavilion at ASU, Tempe), hosted by GDG Phoenix and GDG on Campus ASU–Tempe with sunhacks.

Two hand-written pages, no build step: `index.html` (home, compact schedule) and `schedule.html` (expanded
schedule with speaker cards), sharing `site.css`. Edit, commit, push. GitHub Pages serves the repo root;
`CNAME` keeps the custom domain. DNS is on Cloudflare (apex A/AAAA to GitHub Pages, `www` CNAME to
tooshel.github.io, all DNS-only).

- RSVP goes to the GDG community event page; the call for speakers (Sessionize/Advocu) closed Oct 28.
- `devfest-phoenix-2026.ics`: add-to-calendar file (9 AM–6:20 PM Arizona = 16:00–01:20 UTC).
- `img/og.png`: social share image, rendered from HTML with headless Chrome.
- "Getting there" map (`#venue`): Leaflet 1.9.4 vendored in `vendor/leaflet/`, lazy-loaded when the map nears
  view, OpenStreetMap tiles. Pin coordinates come from OpenStreetMap; the walking route line is from
  routing.openstreetmap.de (foot profile). Parking: Apache Blvd Parking Structure (paid on weekends);
  check-in 9 AM at the Student Pavilion; talks from 10 AM in LSE 104.
- Schedule (`#schedule`): speakers + talk titles by time slot (titles matched from the prelim list), check-in
  shown as 9–10 AM with a note that it stays open until 11:45. Workshops listed below; their times may change.
- `schedule.html` speaker photos are `img/speakers/<first-last>.jpg` (200px square, shown as 52px circles).
  Photos and talk/role/bio text came from the organizers' Figma speaker page (xYNdGQ1RFPyaGqL04Rh2n8); the
  images were pulled from the file's image fills and matched to speakers by eye.
