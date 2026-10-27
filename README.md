# LeadGen Demo Site: Northside Plumbing

A demo website for **Northside Plumbing**, a made-up family plumber in Spokane, WA. The business, people, address, phone number and reviews are all fictional.

It shows what LeadGen does for a client. We take a local business that already has a good reputation (hundreds of strong Google reviews, years of word-of-mouth customers) but almost nothing online, and we give it a web presence that customers and AI search tools can actually find.

## What's in it

The essay said a business needs "a clear website with a page for each service." Here's what we built for that:

- **One page per service.** There are pages for water heaters, drains, leaks, frozen pipes, repiping and sewer lines. Each one covers the signs of the problem, what we do, a rough price, and common questions, written in the owner's voice.
- **Phone number on every page.** It's in the header and footer, and on phones a "Call" bar stays pinned to the bottom of the screen.
- **Real local detail.** Neighborhoods, the age of Spokane's housing, our winters. This is what separates a real local business from a generic template, for people and for search engines alike.
- **Structured business data.** The home page includes Schema.org `Plumber` data (name, address, phone, hours, service area). Google and AI assistants read this to understand who the business is.
- **Reviews out front.** Reviews show up on the home page and have their own page, which also asks past customers to leave a new one.
- **Real photos.** There are 20 photos, including real Spokane neighborhoods (South Hill, Browne's Addition, Perry District, Hillyard) and plumbing work. All come from Wikimedia Commons under free licenses, are resized into `assets/images/`, and are credited on `pages/credits.html`.

## How the files are organized

```
index.html          Home page (has to stay at the root for GitHub Pages)
services/           One page per service: water heaters, drains, leaks, frozen pipes, repiping, sewer lines
pages/              About, reviews, contact, photo credits
assets/styles.css   The one stylesheet every page uses
assets/favicon.svg  Browser tab icon
assets/images/      All 20 photos
```

## Demo-only details

A real client site would drop all of these:

- A banner on every page says the business is fictional.
- Every page has `<meta name="robots" content="noindex">` so search engines don't list a fake business.
- The phone number uses the 555-01xx range, which is reserved for fiction.
- The contact form and the "Leave a Google review" button show a demo message instead of sending anything.

## Viewing it

Open `index.html` in a browser. It's plain HTML and CSS, with no build step and nothing to install.

## Publishing on GitHub Pages

1. Push to `main`.
2. On GitHub, go to **Settings > Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, then select `main` and `/ (root)`.
4. After a minute or two, the site will be live at `https://nickvlasceanu.github.io/LeadGenDemoSite/`.

By Nick Vlasceanu and Braden Calme.
