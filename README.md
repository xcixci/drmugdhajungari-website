# drmugdhajungari.in

Website for Dr Mugdha Jungari and The Purple Women's Health Clinic, Nagpur.
Plain HTML and CSS, no build step. Everything that goes live is in the `site/` folder.

## Publish on Netlify

1. In Netlify: **Add new site → Import an existing project → GitHub** and pick this repo.
2. Netlify reads `netlify.toml`, so the publish folder (`site`) is already set. No build command.
3. **Domain management → Add a domain**: `www.drmugdhajungari.in` (and the bare domain, which redirects to www).
4. At the domain registrar, point the DNS to Netlify as Netlify shows you. HTTPS switches on by itself.
5. After it's live, add `https://www.drmugdhajungari.in/` as the website on her Google Business Profile.

Every push to `main` republishes the site automatically.

## Things to fill in before launch

All marked with comments in `site/index.html` (search for the capitalised word):

| Search for | What to do |
|---|---|
| `BOOKING LINK` | Replace `tel:+918767497629` with her booking link and change the button text to "Book an appointment". |
| `REGISTRATION NUMBER` | Remove the comment marks around the block and add her Maharashtra Medical Council number. |
| `WHATSAPP` | Confirm +91 87674 97629 is on WhatsApp. If not, delete both WhatsApp links. |
| `ANALYTICS` | Paste a cookie-free analytics script (for example Umami). Calls, WhatsApp, directions and Instagram taps are already tagged, so you can show her how many patients the site sends. |
| `PHOTO` | If she or her agency prefers no photo in the top section under the NMC advertising guidelines (Oct 2026), delete the marked `<figure>` block. Her name still fills the top of the page. |

## Facts to confirm with Dr Mugdha

Taken from her Wix demo, Google Business Profile and public listings:

- 19 years of practice
- Principal Consultant, Obstetrics & Gynaecology, Max Super Speciality Hospital, Nagpur
- MBBS, MUHS, 2007; MS, Grant Medical College and Sir JJ Hospital, Mumbai, 2012
- Postgraduate teaching and NMC curriculum work
- Partners welcome at consultations
- Life member of NOGS, IAGE and the PCOS Society of India
- Instagram: @thepurplewomenshealthclinic
- She is happy for the site to use: the first-visit video (from Instagram; ask for the original file, it will look sharper), the Max photo, the G H Raisoni College talk photo and the Lokmat Times article
- Captions in "Teaching, talks and writing" are accurate
- First-visit section: what to bring (reports and scans, prescriptions and current medicines, date of last period) and how a consultation goes

## Rules this site follows (NMC ethical advertising guidelines, 6 Oct 2026)

- No patient testimonials or reviews, real or AI-generated, even with consent.
- No "best", "No. 1", success rates or guaranteed outcomes.
- Facts only: qualifications, roles, services, address, hours, phone.
- No photos with pharma or product branding (the podium photo is cropped to remove it), and no identifiable students or patients.

Keep it that way when editing.

## Files

- `site/index.html` – the page, including structured data (schema.org) that Google and AI tools read
- `site/privacy.html`, `site/404.html`
- `site/assets/css/site.css` – all styles
- `site/assets/fonts/` – Gloock and Figtree, self-hosted
- `site/assets/img/` – logo mark, BirthWise logo, photo, link-preview image
- `site/robots.txt`, `site/sitemap.xml`, `site/_headers`

Built by Arinjay Business Systems.
