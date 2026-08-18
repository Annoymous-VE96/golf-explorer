# Golf Explorer - Homepage Redesign Template

## 1. Design System Tokens (CSS Variables)
- **Theme:** Luxury Travel, High-End Golf Vacations, Authoritative & Elegant.
- **Color Palette (Map to CSS :root):**
  - `--primary-color`: Deep Forest Green (`#1E3F20`) - Navigation, primary actions, deep footers.
  - `--secondary-color`: Warm Sand (`#F5F5F0`) - Alternate row section backgrounds, background cards.
  - `--accent-color`: Champagne Gold (`#C5A880`) - Highlights, star ratings, hover borders, subtle glowing accents.
  - `--text-dark`: Charcoal (`#1F2937`) - High contrast body text.
  - `--text-light`: Pure White (`#FFFFFF`) - Overlaid hero text and dark section contrast.
- **Typography Scale:**
  - **Serif Headings:** `Playfair Display` or `Merriweather` via Google Fonts (H1: 3.5rem/4.5rem, H2: 2.25rem, H3: 1.5rem)
  - **Sans-serif Body:** `Inter` or `Montserrat` via Google Fonts (Body: 1rem/1.125rem, UI/Nav: 0.875rem tracking-wide)
- **Animation System (Vanilla CSS/JS):**
  - **Card Hover:** `transform: translateY(-4px)`, `box-shadow` transition, subtle border glow.
  - **Scroll Reveal:** `opacity: 0; transform: translateY(20px);` transitioning to `opacity: 1; transform: translateY(0);` via JS Intersection Observer adding an `.is-visible` class.

---

## 2. Section Hierarchy & Structural Blueprint

### Section 1: Sticky Navigation Header (`<header>`)
- **Layout:** Sticky top navigation bar. Starts transparent on hero top, transitions to solid white backdrop with subtle shadow via Vanilla JS on scroll.
- **Left:** Golf Explorer Brand Logo.
- **Center:** Navigation Links: `About us`, `Reviews`, `Blogs`, `Contact`. (Active/hover state: Gold underline transition).
- **Right:** Phone Link (`+61 8 8376 4495`) + Primary CTA Button ("Browse Packages").
- **Mobile:** Include a JS-toggled Hamburger Menu.

### Section 2: Premium Hero Banner (`<section id="hero">`)
- **Visuals:** Full-width hero viewport (min-height: 85vh) featuring a stunning, sun-drenched coastal golf course background image.
- **Overlay:** Dual linear gradient overlay in CSS (Dark overlay left-to-right & bottom-to-top) for peak legibility.
- **Content:**
  - **Eyebrow Tag:** "AUSTRALIAN GOLF TRAVEL SPECIALISTS"
  - **H1:** "Golf Holiday Deals & Tour Packages in Australia & Worldwide"
  - **Sub-headline:** "Crafting memorable golf holidays tailored to your exact needs."
  - **CTA Group:** Primary button ("Explore Golf Holidays").

### Section 3: Brand Introduction & Trust Signals (`<section id="intro">`)
- **Layout:** 2-column CSS Grid/Flexbox desktop / 1-column mobile. Sand background (`var(--secondary-color)`).
- **Left Column:**
  - **H2:** "Welcome to Golf Explorer!"
  - **Body:** "We are the Australian golf travel specialists, passionate about crafting memorable golf holidays for our clients. Whether you're looking for a golf holiday to Australia or New Zealand, or indeed to any other country in the world, we can tailor a package to suit your needs. Our personalised and dedicated service is what brings clients back year after year."
- **Right Column (PGA Director Endorsement Card):**
  - **Card UI:** Elevated white card with soft shadow.
  - **Rating:** 5 Gold Stars.
  - **Quote:** “I'd recommend Golf Explorer's services to anyone. You and your team did a terrific job. It was one of the best adventures our group has ever enjoyed!"
  - **Author:** Jim Smith, PGA Director of Golf, The Philadelphia Cricket Club.

### Section 4: Featured Golf Packages (`<section id="packages">`)
- **Layout:** Categorized 3-column responsive CSS Grid.
- **Section Heading:** "Featured Destinations & Curated Packages"

#### Category A: NZ Golf Holidays
- **Card 1:** Title: North Island Golf Tour, New Zealand | Duration: 7 nights | Price: from AU$3,598.00 per person
- **Card 2:** Title: Queenstown Lakefront Villa Golf Retreat | Duration: 7 nights | Price: from AU$4,365.00 per person

#### Category B: Adelaide Golf & Wine
- **Card 3:** Title: The Barossa Beauty | Duration: 7 nights | Price: from AU$3,588.00 per person
- **Card 4:** Title: LIV Golf Experience | Duration: 6 nights | Price: from AU$3,245.00 per person

#### Category C: Australian Golf Breaks
- **Card 5:** Title: Barnbougle Golf Break | Duration: 3 nights | Price: from AU$1,068.00 per person
- **Card 6:** Title: Hamilton Island Golf Break | Duration: 4 nights | Price: from AU$1,228.00 per person
- **Card 7:** Title: Mornington Peninsula Short | Duration: 3 nights | Price: from AU$769.00 per person

### Section 5: The Explorer's Promise (`<section id="features">`)
- **Layout:** 3-column Flexbox feature cards.
- **Card 1 (Where can we take you?):** "With the growing popularity of golf vacations, experience golf breaks in most countries... From New Zealand, Fiji and Vietnam to South Africa, Canada and the links of Scotland and Ireland, we can arrange the most spectacular golf getaways."
- **Card 2 (Play the best golf courses…):** "Whether you're playing the iconic (Pebble Beach, TPC Sawgrass, Old Course St. Andrews) or the spectacular (Cape Kidnappers, Natadola Bay), the world of golf course design is constantly evolving."
- **Card 3 (Call us now…):** "The next step is yours. Browse our website to whet your appetite, or if you prefer to chat, call us on +61 8 8376 4495 or email info@golfexplorer.com.au."

### Section 6: Newsletter Subscription (`<section id="newsletter">`)
- **Layout:** Full-width Forest Green banner.
- **Copy:** H2: "Subscribe for news & promotions"
- **Form UI:** Inline HTML form with inputs for Name, Email, and a Champagne Gold "Subscribe" CTA button.

### Section 7: Global Footer (`<footer>`)
- **Layout:** 4-Column desktop layout in Dark Charcoal background.
- **Column 1:** Golf Explorer Brand, TTA 208954 | Travel Agent Licence.
- **Column 2:** Navigation Links (Sitemap, Privacy & Disclaimer).
- **Column 3:** Contact details (+61 8 8376 4495, info@golfexplorer.com.au).
- **Column 4:** Accreditation badges (IAGTO logo, TCF logo).
- **Bottom Bar:** Copyright notice + Social media icons.
