# Session 01 — DEOSAI Expeditions (Travel Tips & Safety Page)

- **Conversation ID:** `cd531357-fa2a-4237-8674-3e52464aafff`
- **Date:** 2026-11-28

---

## User (2026-11-28T08:17:14Z)

# Project Task: Develop the Travel Tips & Safety Page – DEOSAI Expeditions

I am working on a university IICT website project called DEOSAI Expeditions. My task is to develop a professional, fully responsive Travel Tips & Safety page as an integral part of the existing website.

The objective is to design and implement this page using the existing website architecture, shared CSS stylesheet, JavaScript functionality, typography, colors and design conventions.

## Development Approach

First, inspect the existing project files and understand the website's architecture.

Study the homepage and other existing pages to identify:

- Website branding and visual identity.
- Navbar and footer structure.
- Color palette and typography.
- Existing Bootstrap components.
- Shared CSS classes.
- Existing JavaScript functionality.
- Directory structure and relative file paths.

Then plan and implement the Travel Tips & Safety page following the same design system.

The page must feel like a natural, professionally designed part of DEOSAI Expeditions.

## Implementation Requirements

Develop the page with the following sections:

1. Top Contact & Safety Information Strip.
2. Responsive Main Navigation Bar.
3. Travel Tips & Safety Hero Section.
4. Six Travel Advisory Information Cards:
   - Pakistan Online e-Visa.
   - NOC & Restricted Areas.
   - SCOM SIM Card (Telecom).
   - Currency & ATMs.
   - Altitude Health (AMS).
   - Packing & Dress Etiquette.
5. Safety & Logistics FAQs with a functional Bootstrap accordion containing three questions.
6. Consistent Website Footer.
7. Floating WhatsApp Contact Button.

Use the complete content and descriptions specified in the project requirements.

## Technical Integration

- HTML5 and Bootstrap 5.3.3.
- Bootstrap Icons 1.11.3.
- Existing Google Fonts.
- Existing shared `css/style.css`.
- Existing shared `js/main.js`.
- Correct relative paths according to the project directory.
- Existing reusable website classes and components.
- Responsive Bootstrap grid system.

Do not introduce conflicting global CSS or duplicate JavaScript functionality.

Do not unnecessarily modify other pages or shared files.

## Quality Assurance

After development, verify:

- Responsive layouts.
- Navigation and dropdown functionality.
- FAQ accordion functionality.
- Currency switch compatibility.
- Correct internal links.
- CSS and JavaScript loading.
- Consistent website branding.
- Compatibility with the existing website.

Keep the implementation organized, understandable and appropriate for a university IICT project.

Finally, summarize the implementation, identify modified files and report the testing performed.

---

## User (2026-11-28T08:21:32Z)

you are only required to make the tips page for now, the remaining pages are for later. your task for now is only to create the tips page

---

## Assistant (2026-11-28T08:22:59Z)

Before I create or modify `tips.html`, I inspected your system to locate the existing DEOSAI Expeditions project files and found a few important gaps:

### What I Found
In `C:\Users\HAROON TRADERS\Downloads\`, the following DEOSAI Expeditions HTML pages exist:
- [blog.html](file:///C:/Users/HAROON%20TRADERS/Downloads/blog.html)
- [contact.html](file:///C:/Users/HAROON%20TRADERS/Downloads/contact.html)
- [reviews.html](file:///C:/Users/HAROON%20TRADERS/Downloads/reviews.html)
- [tips.html](file:///C:/Users/HAROON%20TRADERS/Downloads/tips.html) and [tips (1).html](file:///C:/Users/HAROON%20TRADERS/Downloads/tips%20(1).html) (two identical copies already containing a Travel Tips & Safety layout)

### What Is Missing
- There is no active workspace open, and the shared DEOSAI Expeditions files referenced by those pages—`../css/style.css`, `../js/main.js`, `../index.html`, and the other `pages/*.html` files—are not present on your local drives (`Downloads\index.html` and `Downloads\style.css` belong to an unrelated "Plain Cake" file).
- Without `css/style.css`, `js/main.js`, and `index.html`, I can match the HTML structure and CSS classes used in [blog.html](file:///C:/Users/HAROON%20TRADERS/Downloads/blog.html), [contact.html](file:///C:/Users/HAROON%20TRADERS/Downloads/contact.html), and [reviews.html](file:///C:/Users/HAROON%20TRADERS/Downloads/reviews.html), but I cannot directly verify custom stylesheet rendering or `main.js` currency-switch behavior against the live assets.

### How Would You Like to Proceed?
1. **Open/share the project folder:** If `index.html`, `css/style.css`, and `js/main.js` are in another folder or repo, please open that folder as the workspace (or share its path) so I can inspect the shared CSS/JS and place `tips.html` directly inside `pages/`.
2. **Create only `tips.html` now:** If you don't have the rest of the project locally yet, let me know where to write `tips.html` (for example, `C:\Users\HAROON TRADERS\.gemini\antigravity\scratch\deosai-expeditions\pages\tips.html` or updating `Downloads\tips.html`) and whether you want a fresh implementation or specific improvements over the existing [tips.html](file:///C:/Users/HAROON%20TRADERS/Downloads/tips.html) in `Downloads`.

---

## User (2026-11-28T08:28:18Z)

these are the js and css files that were originally made , now this page should be made according to the css and java files and remember that whatever classes and id you give to objects it should be according to the main css and java files

### Attached File (`text/javascript`)

```javascript
/**
 * DEOSAI EXPEDITIONS - Master Interactive Engine
 * Featuring:
 * 1. GoWander Arched Curved Destination Carousel (Exact Reference Implementation)
 * 2. Background Crossfade & Headline Synchronization
 * 3. Dual-Currency Switcher (PKR ₨ ⇄ USD $)
 * 4. High-Contrast Trip Cost Calculator
 */

document.addEventListener('DOMContentLoaded', () => {
  initArchedHeroCarousel();
  initCurrencySwitcher();
  initTripCalculator();
  initNavbarScroll();
  initTourFilters();
  initBookingPage();
  initPlannerForm();
});

/* ==========================================================================
   1. The GoWander-Style Arched Curved Carousel Engine
   ========================================================================== */
const DESTINATIONS = [
  {
    id: 0,
    title: "Passu Cones",
    subtitle: "Cathedral peaks towering over the ancient Silk Road, Attabad Lake, and apricot orchards.",
    location: "Hunza Valley, Gilgit-Baltistan",
    rating: "★ 4.98 (340+ Reviews)",
    link: "pages/hunza.html",
    bg: "https://images.unsplash.com/photo-1544735716-392fe2489ffa?auto=format&fit=crop&w=1920&q=80",
    thumb: "https://images.unsplash.com/photo-1544735716-392fe2489ffa?auto=format&fit=crop&w=400&q=80",
    elevation: "2,500m"
  },
  {
    id: 1,
    title: "Deosai Plains",
    subtitle: "The Land of Giants. Earth's second-highest plateau of wildflowers, Sheosar Lake, and brown bears.",
    location: "Skardu & Baltistan",
    rating: "★ 4.96 (280+ Reviews)",
    link: "pages/skardu.html",
    bg: "https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1920&q=80",
    thumb: "https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=400&q=80",
    elevation: "4,114m"
  },
  {
    id: 2,
    title: "Fairy Meadows",
    subtitle: "Cliffside jeep tracks climbing to pine-scented meadows beneath the 8,126m ice wall of Nanga Parbat.",
    location: "Diamer District, Gilgit-Baltistan",
    rating: "★ 4.99 (410+ Reviews)",
    link: "pages/fairy-meadows.html",
    bg: "https://images.unsplash.com/photo-1464822759023-fed622ff2c3b?auto=format&fit=crop&w=1920&q=80",
    thumb: "https://images.unsplash.com/photo-1464822759023-fed622ff2c3b?auto=format&fit=crop&w=400&q=80",
    elevation: "3,300m"
  },
  {
    id: 3,
    title: "Chitral & Kalash",
    subtitle: "Ancient Kalash valleys, vibrant seasonal festivals, Shandur Polo Pass, and the shadow of Tirich Mir.",
    location: "Hindu Kush, Khyber Pakhtunkhwa",
    rating: "★ 4.95 (220+ Reviews)",
    link: "pages/chitral.html",
    bg: "https://images.unsplash.com/photo-1519681393784-d120267933ba?auto=format&fit=crop&w=1920&q=80",
    thumb: "https://images.unsplash.com/photo-1519681393784-d120267933ba?auto=format&fit=crop&w=400&q=80",
    elevation: "3,700m"
  },
  {
    id: 4,
    title: "Swat & Kalam",
    subtitle: "The Switzerland of the East. Crystal alpine lakes, cedar forests, Malam Jabba ski slopes, and Buddhist relics.",
    location: "Khyber Pakhtunkhwa",
    rating: "★ 4.92 (310+ Reviews)",
    link: "pages/swat.html",
    bg: "https://images.unsplash.com/photo-1507525428034-b723cf961d3e?auto=format&fit=crop&w=1920&q=80",
    thumb: "https://images.unsplash.com/photo-1507525428034-b723cf961d3e?auto=format&fit=crop&w=400&q=80",
    elevation: "2,000m"
  }
];

let activeIndex = 0;
const TOTAL = DESTINATIONS.length;

function initArchedHeroCarousel() {
  const cards = document.querySelectorAll('.curved-card');
  const bgLayers = document.querySelectorAll('.hero-bg-layer');

  if (!cards.length) return;

  cards.forEach(card => {
    card.addEventListener('click', () => {
      const targetIndex = parseInt(card.dataset.index, 10);
      if (targetIndex === activeIndex) {
        // Center card was clicked: directly open its unique themed destination page!
        const dest = DESTINATIONS[targetIndex];
        if (dest && dest.link) {
          window.location.href = dest.link;
        }
      } else {
        // Rotate this card into the center slot
        setActiveDestination(targetIndex);
      }
    });
  });

  // Carousel Arrow Navigation Buttons
  const prevBtn = document.querySelector('.carousel-nav-btn.prev-btn');
  const nextBtn = document.querySelector('.carousel-nav-btn.next-btn');
  if (prevBtn) {
    prevBtn.addEventListener('click', (e) => {
      e.stopPropagation();
      setActiveDestination((activeIndex - 1 + TOTAL) % TOTAL);
    });
  }
  if (nextBtn) {
    nextBtn.addEventListener('click', (e) => {
      e.stopPropagation();
      setActiveDestination((activeIndex + 1) % TOTAL);
    });
  }

  // Keyboard navigation (Left / Right arrows, Enter to open)
  window.addEventListener('keydown', (e) => {
    if (e.key === 'ArrowRight') {
      setActiveDestination((activeIndex + 1) % TOTAL);
    } else if (e.key === 'ArrowLeft') {
      setActiveDestination((activeIndex - 1 + TOTAL) % TOTAL);
    } else if (e.key === 'Enter') {
      const dest = DESTINATIONS[activeIndex];
      if (dest && dest.link) {
        window.location.href = dest.link;
      }
    }
  });

  // Touch Swipe on the carousel track
  const track = document.querySelector('.arched-carousel-wrapper');
  if (track) {
    let touchStartX = 0;
    let touchStartTime = 0;
    track.addEventListener('touchstart', (e) => {
      touchStartX = e.touches[0].clientX;
      touchStartTime = Date.now();
    }, { passive: true });

    track.addEventListener('touchend', (e) => {
      const touchEndX = e.changedTouches[0].clientX;
      const diff = touchStartX - touchEndX;
      const timeDiff = Date.now() - touchStartTime;
      if (Math.abs(diff) > 35 && timeDiff < 600) {
        if (diff > 0) {
          setActiveDestination((activeIndex + 1) % TOTAL);
        } else {
          setActiveDestination((activeIndex - 1 + TOTAL) % TOTAL);
        }
      }
    });
  }

  // Initial setup
  setActiveDestination(0);
}

function setActiveDestination(newIndex) {
  activeIndex = newIndex;
  const cards = document.querySelectorAll('.curved-card');
  const bgLayers = document.querySelectorAll('.hero-bg-layer');
  const titleEl = document.getElementById('hero-title');
  const descEl = document.getElementById('hero-desc');
  const ctaBtn = document.getElementById('hero-cta');
  const locEl = document.getElementById('hero-location');
  const ratingEl = document.getElementById('hero-rating');

  const data = DESTINATIONS[newIndex];
  if (!data) return;

  // 1. Update Arched Card Slots along the smiling curve
  cards.forEach(card => {
    const cardIndex = parseInt(card.dataset.index, 10);
    // Relative position delta: -2, -1, 0, 1, 2
    let delta = (cardIndex - activeIndex + TOTAL) % TOTAL;
    if (delta > 2) delta -= TOTAL;

    // Reset slot classes
    card.className = 'curved-card';

    if (delta === 0) {
      card.classList.add('slot-center');
    } else if (delta === -1) {
      card.classList.add('slot-left');
    } else if (delta === -2) {
      card.classList.add('slot-far-left');
    } else if (delta === 1) {
      card.classList.add('slot-right');
    } else if (delta === 2) {
      card.classList.add('slot-far-right');
    } else {
      card.classList.add('slot-hidden');
    }
  });

  // 2. Crossfade Full-Bleed Background Layer
  bgLayers.forEach((layer, i) => {
    layer.classList.toggle('is-active', i === newIndex);
  });

  // 3. Update Text with smooth slide-up effect
  if (titleEl && descEl && ctaBtn) {
    titleEl.style.opacity = '0';
    titleEl.style.transform = 'translateY(15px)';
    
    setTimeout(() => {
      titleEl.textContent = data.title;
      descEl.textContent = data.subtitle;
      ctaBtn.href = data.link;
      ctaBtn.textContent = `Explore ${data.title} →`;

      titleEl.style.opacity = '1';
      titleEl.style.transform = 'translateY(0)';
    }, 200);
  }

  // 4. Update Top Right Meta Badge
  if (locEl && ratingEl) {
    locEl.textContent = data.location;
    ratingEl.textContent = data.rating;
  }
}

/* ==========================================================================
   2. Dual Currency Switcher (PKR ₨ ⇄ USD $)
   ========================================================================== */
let currentCurrency = 'PKR';
const PKR_RATE = 280;

function initCurrencySwitcher() {
  const btnPKR = document.getElementById('curr-pkr');
  const btnUSD = document.getElementById('curr-usd');

  if (!btnPKR || !btnUSD) return;

  btnPKR.addEventListener('click', () => setCurrency('PKR'));
  btnUSD.addEventListener('click', () => setCurrency('USD'));
}

function setCurrency(curr) {
  currentCurrency = curr;

  const btnPKR = document.getElementById('curr-pkr');
  const btnUSD = document.getElementById('curr-usd');
  if (btnPKR && btnUSD) {
    btnPKR.classList.toggle('active', curr === 'PKR');
    btnUSD.classList.toggle('active', curr === 'USD');
  }

  // Update all elements with data-pkr
  document.querySelectorAll('[data-pkr]').forEach(el => {
    const pkr = parseInt(el.dataset.pkr, 10);
    if (curr === 'PKR') {
      el.textContent = `₨ ${pkr.toLocaleString('en-PK')}`;
    } else {
      const usd = Math.round(pkr / PKR_RATE);
      el.textContent = `$${usd.toLocaleString('en-US')}`;
    }
  });

  // Recalculate trip estimator if present
  if (typeof recalcEstimator === 'function') {
    recalcEstimator();
  }
}

/* ==========================================================================
   3. Trip Cost Estimator
   ========================================================================== */
let estState = {
  days: 7,
  guests: 4,
  vehicle: 'prado',
  tier: 'boutique'
};

const VEHICLE_PRICES = { corolla: 14000, prado: 26000, hiace: 22000 };
const HOTEL_PRICES = { alpine: 6500, boutique: 14500, luxury: 28000 };

function initTripCalculator() {
  const daysSlider = document.getElementById('est-days-slider');
  const guestsSlider = document.getElementById('est-guests-slider');
  const daysLabel = document.getElementById('est-days-label');
  const guestsLabel = document.getElementById('est-guests-label');

  if (!daysSlider || !guestsSlider) return;

  daysSlider.addEventListener('input', (e) => {
    estState.days = parseInt(e.target.value, 10);
    if (daysLabel) daysLabel.textContent = `${estState.days} Days`;
    recalcEstimator();
  });

  guestsSlider.addEventListener('input', (e) => {
    estState.guests = parseInt(e.target.value, 10);
    if (guestsLabel) guestsLabel.textContent = `${estState.guests} Guests`;
    recalcEstimator();
  });

  document.querySelectorAll('[data-opt-vehicle]').forEach(btn => {
    btn.addEventListener('click', () => {
      document.querySelectorAll('[data-opt-vehicle]').forEach(b => b.classList.remove('active'));
      btn.classList.add('active');
      estState.vehicle = btn.dataset.optVehicle;
      recalcEstimator();
    });
  });

  document.querySelectorAll('[data-opt-tier]').forEach(btn => {
    btn.addEventListener('click', () => {
      document.querySelectorAll('[data-opt-tier]').forEach(b => b.classList.remove('active'));
      btn.classList.add('active');
      estState.tier = btn.dataset.optTier;
      recalcEstimator();
    });
  });

  recalcEstimator();
}

function recalcEstimator() {
  const vehicleCost = estState.days * VEHICLE_PRICES[estState.vehicle];
  const hotelCost = estState.days * estState.guests * HOTEL_PRICES[estState.tier];
  const logistics = estState.days * 4500;

  const totalPKR = vehicleCost + hotelCost + logistics;
  const perPersonPKR = Math.round(totalPKR / estState.guests);

  const totalDisplay = document.getElementById('est-total-out');
  const perPersonDisplay = document.getElementById('est-perperson-out');
  const waBtn = document.getElementById('est-whatsapp-btn');

  if (totalDisplay && perPersonDisplay) {
    if (currentCurrency === 'PKR') {
      totalDisplay.innerHTML = `<span>₨</span> ${totalPKR.toLocaleString('en-PK')}`;
      perPersonDisplay.textContent = `Approx. ₨ ${perPersonPKR.toLocaleString('en-PK')} / person`;
    } else {
      const totalUSD = Math.round(totalPKR / PKR_RATE);
      const perPersonUSD = Math.round(totalUSD / estState.guests);
      totalDisplay.innerHTML = `<span>$</span> ${totalUSD.toLocaleString('en-US')}`;
      perPersonDisplay.textContent = `Approx. $${perPersonUSD.toLocaleString('en-US')} / person`;
    }
  }

  if (waBtn) {
    const vNames = { corolla: 'Sedan Corolla', prado: 'Toyota Prado 4x4', hiace: 'Grand Cabin HiAce' };
    const tNames = { alpine: 'Standard Lodges', boutique: 'Boutique Resorts', luxury: 'Heritage Forts' };

    const text = encodeURIComponent(
      `Salam DEOSAI Expeditions! I configured this trip on your website:\n\n` +
      `• Duration: ${estState.days} Days\n` +
      `• Travelers: ${estState.guests} Guests\n` +
      `• Dedicated 4x4: ${vNames[estState.vehicle]}\n` +
      `• Hotel Tier: ${tNames[estState.tier]}\n` +
      `• Estimated Investment: ₨ ${totalPKR.toLocaleString('en-PK')}\n\n` +
      `Please send me the complete day-by-day itinerary schedule!`
    );
    waBtn.href = `https://wa.me/923000000000?text=${text}`;
  }
}

function initNavbarScroll() {
  const nav = document.querySelector('.navbar-alpine');
  if (!nav) return;
  window.addEventListener('scroll', () => {
    if (window.scrollY > 40) {
      nav.classList.add('scrolled');
    } else {
      nav.classList.remove('scrolled');
    }
  }, { passive: true });
}

/* ==========================================================================
   4. Tour Packages Filter Pills (pages/packages.html)
   ========================================================================== */
function initTourFilters() {
  const pills = document.querySelectorAll('.tour-filter-pill');
  const items = document.querySelectorAll('.tour-filter-item');
  if (!pills.length || !items.length) return;

  pills.forEach(pill => {
    pill.addEventListener('click', () => {
      const filter = pill.dataset.filter;
      pills.forEach(p => {
        p.classList.remove('active', 'btn-pine');
        p.classList.add('btn-pine-outline');
      });
      pill.classList.add('active', 'btn-pine');
      pill.classList.remove('btn-pine-outline');

      items.forEach(item => {
        const match = filter === 'all' || item.dataset.category === filter;
        item.style.display = match ? '' : 'none';
      });
    });
  });
}

/* ==========================================================================
   5. Booking & WhatsApp Pre-fill Engine (pages/contact.html)
   ========================================================================== */
function initBookingPage() {
  const form = document.getElementById('booking-inquiry-form');
  if (!form) return;

  const params = new URLSearchParams(window.location.search);
  const tour = params.get('tour');
  const plan = params.get('plan');

  const banner = document.getElementById('selected-tour-banner');
  const bannerTitle = document.getElementById('selected-tour-name');
  const subjectEl = document.getElementById('booking-subject');
  const messageEl = document.getElementById('booking-message');
  const waBtn = document.getElementById('whatsapp-booking-btn');

  if (tour) {
    if (banner && bannerTitle) {
      bannerTitle.textContent = tour;
      banner.classList.remove('d-none');
    }
    if (subjectEl) {
      const customOpt = document.createElement('option');
      customOpt.value = `Booking: ${tour}`;
      customOpt.textContent = `Booking: ${tour}`;
      customOpt.selected = true;
      subjectEl.prepend(customOpt);
    }
    if (messageEl && !messageEl.value.trim()) {
      messageEl.value = plan
        ? `I would like to book / finalize my ${tour}:\n${plan}`
        : `I would like to book the "${tour}" package. Please share available dates, group rates, and confirmation steps.`;
    }
    if (waBtn) {
      const waText = encodeURIComponent(
        `Salam DEOSAI Expeditions! I want to book: ${tour}.${plan ? '\n\n' + plan : ''}`
      );
      waBtn.href = `https://wa.me/923000000000?text=${waText}`;
    }
  }

  form.addEventListener('submit', (e) => {
    e.preventDefault();
    const name = (document.getElementById('booking-name')?.value || '').trim();
    const email = (document.getElementById('booking-email')?.value || '').trim();
    const phone = (document.getElementById('booking-phone')?.value || '').trim();
    const subject = (subjectEl?.value || 'Tour Booking').trim();
    const message = (messageEl?.value || '').trim();

    const waSummary = encodeURIComponent(
      `Salam DEOSAI Expeditions!\n\n` +
      `• Name: ${name}\n` +
      `• Phone: ${phone}\n` +
      `• Email: ${email}\n` +
      `• Tour / Subject: ${subject}\n` +
      `• Details: ${message}`
    );
    const waUrl = `https://wa.me/923000000000?text=${waSummary}`;

    const statusBox = document.getElementById('booking-confirmation');
    const statusWa = document.getElementById('booking-confirm-wa');
    if (statusBox && statusWa) {
      statusWa.href = waUrl;
      statusBox.classList.remove('d-none');
      statusBox.scrollIntoView({ behavior: 'smooth', block: 'nearest' });
    }
  });
}

/* ==========================================================================
   6. Custom Trip Planner Forwarder (pages/planner.html)
   ========================================================================== */
function initPlannerForm() {
  const form = document.getElementById('custom-planner-form');
  if (!form) return;

  form.addEventListener('submit', (e) => {
    e.preventDefault();
    const valleys = Array.from(form.querySelectorAll('input[name="valleys"]:checked'))
      .map(cb => cb.value)
      .join(', ') || 'Northern Pakistan';
    const month = form.querySelector('#plan-month')?.value || '';
    const duration = form.querySelector('#plan-duration')?.value || '';
    const guests = form.querySelector('#plan-guests')?.value || '4';
    const vehicle = form.querySelector('#plan-vehicle')?.value || '';
    const tier = form.querySelector('#plan-tier')?.value || '';
    const notes = (form.querySelector('#plan-notes')?.value || '').trim();

    const planSummary =
      `Valleys: ${valleys}\n` +
      `Month: ${month}\n` +
      `Duration: ${duration}\n` +
      `Guests: ${guests}\n` +
      `Vehicle: ${vehicle}\n` +
      `Hotel Tier: ${tier}` +
      (notes ? `\nNotes: ${notes}` : '');

    const target = `contact.html?tour=${encodeURIComponent('Custom Trip Plan (' + duration + ')')}&plan=${encodeURIComponent(planSummary)}`;
    window.location.href = target;
  });
}
```

### Attached File (`text/css`)

```css
/* ==========================================================================
   DEOSAI EXPEDITIONS - High-Contrast Master Design System
   WCAG AAA Compliant & Razor-Sharp Legibility Across All 15 Pages
   ========================================================================== */

:root {
  /* High-Contrast Light Theme Palette */
  --bg-page: #F8FAFC;              /* Clean Glacier White */
  --bg-surface: #FFFFFF;           /* Crisp Pure White Surface */
  --bg-subtle: #F1F5F9;            /* Soft Alpine Mist */
  
  --color-primary: #047857;        /* Deep Karakoram Pine */
  --color-primary-hover: #065F46;
  --color-accent: #0284C7;         /* Glacial Lake Cyan */
  --color-gold: #D97706;           /* Mountain Sun Amber */

  /* Text Contrast - Strictly High Contrast (Never Invisible) */
  --text-main: #0F172A;            /* Deep Jet Slate - Maximum Legibility */
  --text-body: #334155;            /* Solid Dark Slate for paragraphs */
  --text-muted: #64748B;           /* Legible secondary slate */
  --text-inverse: #FFFFFF;         /* Crisp White for Dark/Hero Overlays */

  --border-light: #E2E8F0;
  --border-medium: #CBD5E1;
  --border-primary: rgba(4, 120, 87, 0.3);

  --shadow-sm: 0 2px 8px rgba(15, 23, 42, 0.04);
  --shadow-md: 0 10px 25px rgba(15, 23, 42, 0.07);
  --shadow-lg: 0 20px 40px rgba(15, 23, 42, 0.12);

  --font-heading: 'Plus Jakarta Sans', sans-serif;
  --font-body: 'Inter', sans-serif;
  --font-mono: 'Space Grotesk', monospace;

  --transition-smooth: all 0.4s cubic-bezier(0.16, 1, 0.3, 1);
  --transition-fast: all 0.2s ease;
}

/* Base Reset & Text Legibility */
*, *::before, *::after {
  box-sizing: border-box;
}

body {
  background-color: var(--bg-page);
  color: var(--text-body);
  font-family: var(--font-body);
  overflow-x: hidden;
  line-height: 1.65;
  font-size: 1rem;
}

h1, h2, h3, h4, h5, h6 {
  font-family: var(--font-heading);
  font-weight: 700;
  color: var(--text-main);
  letter-spacing: -0.025em;
  line-height: 1.25;
}

p {
  color: var(--text-body);
  margin-bottom: 1rem;
}

.font-mono {
  font-family: var(--font-mono);
}

.text-pine {
  color: var(--color-primary) !important;
}

.text-amber {
  color: var(--color-gold) !important;
}

/* ==========================================================================
   GLOBAL FIX: OVERRIDE ANY ACCIDENTAL WHITE-ON-WHITE TEXT
   Ensures text is NEVER invisible on light sections
   ========================================================================== */
section:not(.gowander-hero):not(.inner-page-header):not(.footer-clean):not(.footer-deosai) h1,
section:not(.gowander-hero):not(.inner-page-header):not(.footer-clean):not(.footer-deosai) h2,
section:not(.gowander-hero):not(.inner-page-header):not(.footer-clean):not(.footer-deosai) h3,
section:not(.gowander-hero):not(.inner-page-header):not(.footer-clean):not(.footer-deosai) h4,
section:not(.gowander-hero):not(.inner-page-header):not(.footer-clean):not(.footer-deosai) h5,
section:not(.gowander-hero):not(.inner-page-header):not(.footer-clean):not(.footer-deosai) h6 {
  color: var(--text-main) !important;
}

section:not(.gowander-hero):not(.inner-page-header):not(.footer-clean):not(.footer-deosai) p,
section:not(.gowander-hero):not(.inner-page-header):not(.footer-clean):not(.footer-deosai) li,
section:not(.gowander-hero):not(.inner-page-header):not(.footer-clean):not(.footer-deosai) span:not(.badge):not(.btn) {
  color: var(--text-body);
}

/* Aggressive Failsafe: Prevent text-white from causing invisible text on light backgrounds */
body:not(.gowander-hero) .container .text-white:not(.inner-page-header *):not(.footer-clean *):not(.badge):not(.btn):not(.btn *):not(.output-price-box *):not(.curved-card *) {
  color: #0F172A !important;
}
body:not(.gowander-hero) .container .text-light:not(.inner-page-header *):not(.footer-clean *):not(.badge):not(.btn) {
  color: #334155 !important;
}
body:not(.gowander-hero) .container .text-white-50 {
  color: #64748B !important;
}

/* Custom Scrollbar */
::-webkit-scrollbar {
  width: 8px;
}
::-webkit-scrollbar-track {
  background: #F1F5F9;
}
::-webkit-scrollbar-thumb {
  background: #94A3B8;
  border-radius: 4px;
}
::-webkit-scrollbar-thumb:hover {
  background: var(--color-primary);
}

/* ==========================================================================
   NAVIGATION (Solid High-Contrast Navbar Across All Pages)
   ========================================================================== */
.top-contact-strip,
.top-notice-bar {
  background: #064E3B !important;
  color: #E2E8F0 !important;
  font-size: 0.82rem;
  padding: 6px 0;
  font-weight: 500;
}

.top-contact-strip a,
.top-notice-bar a {
  color: #A7F3D0 !important;
  text-decoration: none;
}

.navbar,
.navbar-light,
.navbar-dark,
.navbar-alpine,
.navbar-deosai {
  background: #FFFFFF !important;
  border-bottom: 1px solid var(--border-light) !important;
  padding: 0.85rem 0 !important;
  box-shadow: 0 4px 16px rgba(15, 23, 42, 0.06) !important;
}

.brand-wrapper {
  display: flex;
  align-items: center;
  gap: 12px;
  text-decoration: none;
}

.brand-title-alpine,
.brand-text-main {
  font-family: var(--font-heading);
  font-weight: 800;
  font-size: 1.4rem;
  letter-spacing: 0.06em;
  color: #064E3B !important;
  line-height: 1;
}

.brand-sub-alpine,
.brand-text-sub {
  display: block;
  font-size: 0.62rem;
  font-family: var(--font-mono);
  letter-spacing: 0.22em;
  color: #059669 !important;
  margin-top: 3px;
  font-weight: 700;
}

/* Navbar Links: Guaranteed High-Contrast Jet Slate Across All Configurations */
.navbar .nav-link,
.navbar-dark .navbar-nav .nav-link,
.navbar-light .navbar-nav .nav-link,
.navbar-alpine .navbar-nav .nav-link,
.navbar-deosai .navbar-nav .nav-link,
.navbar-nav .nav-link,
.nav-link-alpine,
.nav-link-deosai {
  color: #0F172A !important;
  font-size: 0.92rem;
  font-weight: 600;
  padding: 0.5rem 0.95rem !important;
  transition: var(--transition-fast);
  border-radius: 8px;
  opacity: 1 !important;
}

.navbar .nav-link:hover,
.navbar-dark .navbar-nav .nav-link:hover,
.navbar-light .navbar-nav .nav-link:hover,
.navbar-alpine .navbar-nav .nav-link:hover,
.navbar-deosai .navbar-nav .nav-link:hover,
.navbar .nav-link.active,
.navbar-dark .navbar-nav .nav-link.active,
.navbar-light .navbar-nav .nav-link.active,
.navbar-alpine .navbar-nav .nav-link.active,
.navbar-deosai .navbar-nav .nav-link.active,
.navbar-nav .nav-link.active,
.nav-link-alpine:hover,
.nav-link-alpine.active,
.nav-link-deosai:hover,
.nav-link-deosai.active {
  color: #047857 !important;
  background: rgba(4, 120, 87, 0.08) !important;
}

.navbar-toggler {
  border: 1px solid var(--border-medium) !important;
  padding: 0.35rem 0.65rem;
}
.navbar-toggler-icon {
  filter: invert(0.2) !important;
}

/* Currency Switcher Pill */
.curr-switch-box,
.currency-pill-box {
  background: #F1F5F9 !important;
  border: 1px solid var(--border-light) !important;
  border-radius: 30px;
  padding: 3px;
  display: inline-flex;
}

.curr-pill-btn,
.curr-btn {
  background: transparent;
  border: none;
  color: var(--text-muted) !important;
  font-size: 0.78rem;
  font-weight: 700;
  padding: 4px 10px;
  border-radius: 20px;
  cursor: pointer;
  transition: var(--transition-fast);
}

.curr-pill-btn.active,
.curr-btn.active {
  background: #047857 !important;
  color: #FFFFFF !important;
  box-shadow: 0 2px 6px rgba(4, 120, 87, 0.3) !important;
}

/* Primary Buttons */
.btn-pine,
.btn-emerald {
  background: #047857 !important;
  color: #FFFFFF !important;
  font-family: var(--font-heading);
  font-weight: 700;
  font-size: 0.92rem;
  padding: 0.75rem 1.6rem;
  border-radius: 30px;
  border: none;
  text-decoration: none;
  display: inline-flex;
  align-items: center;
  gap: 8px;
  transition: var(--transition-smooth);
  box-shadow: 0 4px 14px rgba(4, 120, 87, 0.25);
}

.btn-pine:hover,
.btn-emerald:hover {
  background: #065F46 !important;
  color: #FFFFFF !important;
  transform: translateY(-2px);
  box-shadow: 0 8px 22px rgba(4, 120, 87, 0.35);
}

.btn-pine-outline,
.btn-emerald-outline {
  background: #FFFFFF !important;
  color: #047857 !important;
  border: 1.5px solid #047857 !important;
  font-family: var(--font-heading);
  font-weight: 700;
  font-size: 0.92rem;
  padding: 0.75rem 1.6rem;
  border-radius: 30px;
  text-decoration: none;
  display: inline-flex;
  align-items: center;
  gap: 8px;
  transition: var(--transition-smooth);
}

.btn-pine-outline:hover,
.btn-emerald-outline:hover {
  background: rgba(4, 120, 87, 0.08) !important;
  color: #065F46 !important;
  transform: translateY(-2px);
}

/* ==========================================================================
   THE GOWANDER-STYLE ARCHED CAROUSEL HERO SECTION
   ========================================================================== */
.gowander-hero {
  position: relative;
  min-height: 90vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  padding: 90px 0 35px 0;
  overflow: hidden;
  color: #FFFFFF;
}

.hero-bg-canvas {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 0;
}

.hero-bg-layer {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-size: cover;
  background-position: center;
  opacity: 0;
  transition: opacity 0.8s ease, transform 1.2s ease;
  transform: scale(1.05);
}

.hero-bg-layer.is-active {
  opacity: 1;
  transform: scale(1);
}

.hero-gradient-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(180deg, rgba(15, 23, 42, 0.55) 0%, rgba(15, 23, 42, 0.25) 50%, rgba(15, 23, 42, 0.85) 100%);
  pointer-events: none;
  z-index: 1;
}

.hero-text-content {
  position: relative;
  z-index: 2;
}

.hero-title-giant {
  font-size: clamp(3rem, 6.5vw, 5.2rem);
  font-weight: 900;
  line-height: 1;
  letter-spacing: -0.04em;
  color: #FFFFFF !important;
  margin-bottom: 1rem;
  text-shadow: 0 4px 20px rgba(0, 0, 0, 0.6);
  transition: opacity 0.4s ease, transform 0.4s ease;
}

.hero-desc-text {
  font-size: 1.15rem;
  color: rgba(255, 255, 255, 0.95) !important;
  max-width: 540px;
  text-shadow: 0 2px 10px rgba(0, 0, 0, 0.7);
  margin-bottom: 1.8rem;
  line-height: 1.6;
}

.hero-meta-badge {
  position: relative;
  z-index: 2;
  text-align: end;
  background: rgba(15, 23, 42, 0.65);
  backdrop-filter: blur(12px);
  padding: 14px 22px;
  border-radius: 18px;
  border: 1px solid rgba(255, 255, 255, 0.2);
  display: inline-block;
}

.hero-meta-stars {
  color: #FBBF24;
  font-size: 1rem;
}

.hero-meta-location {
  font-family: var(--font-mono);
  font-size: 0.88rem;
  font-weight: 700;
  color: #FFFFFF;
  margin-top: 4px;
}

/* The Curved Carousel Track */
.arched-carousel-wrapper {
  position: relative;
  z-index: 10;
  width: 100%;
  height: 290px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-top: auto;
  user-select: none;
}

.arched-carousel-track {
  position: relative;
  width: 900px;
  height: 270px;
  display: flex;
  align-items: center;
  justify-content: center;
}

/* Navigation Arrow Controls */
.carousel-nav-btn {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  width: 46px;
  height: 46px;
  border-radius: 50%;
  background: rgba(15, 23, 42, 0.7);
  backdrop-filter: blur(12px);
  border: 1.5px solid rgba(255, 255, 255, 0.35);
  color: #FFFFFF;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.25rem;
  cursor: pointer;
  z-index: 25;
  transition: all 0.25s cubic-bezier(0.16, 1, 0.3, 1);
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.4);
}

.carousel-nav-btn:hover {
  background: #047857;
  border-color: #34D399;
  color: #FFFFFF;
  transform: translateY(-50%) scale(1.12);
  box-shadow: 0 10px 25px rgba(4, 120, 87, 0.6);
}

.carousel-nav-btn.prev-btn {
  left: calc(50% - 460px);
}

.carousel-nav-btn.next-btn {
  right: calc(50% - 460px);
}

.curved-card {
  position: absolute;
  width: 175px;
  height: 240px;
  border-radius: 22px;
  overflow: hidden;
  cursor: pointer;
  background: #0F172A;
  box-shadow: 0 15px 35px rgba(0, 0, 0, 0.5);
  transition: all 0.55s cubic-bezier(0.16, 1, 0.3, 1);
  transform-origin: center bottom;
}

.curved-card img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.6s ease;
}

.curved-card:hover img {
  transform: scale(1.08);
}

.curved-card-overlay {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: linear-gradient(180deg, rgba(0,0,0,0.1) 0%, transparent 40%, rgba(0, 0, 0, 0.88) 100%);
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  padding: 16px;
  color: #FFFFFF;
}

.curved-card-title {
  font-family: var(--font-heading);
  font-weight: 800;
  font-size: 1.05rem;
  line-height: 1.2;
  margin: 0;
  color: #FFFFFF !important;
  text-shadow: 0 2px 6px rgba(0, 0, 0, 0.8);
}

.curved-card-alt {
  font-family: var(--font-mono);
  font-size: 0.72rem;
  color: #A7F3D0;
  font-weight: 600;
}

/* Enter Valley Pill Badge on Active Card */
.curved-card .enter-valley-badge {
  display: none;
  background: #047857;
  color: #FFFFFF;
  font-size: 0.74rem;
  font-weight: 700;
  padding: 5px 12px;
  border-radius: 20px;
  margin-top: 8px;
  align-items: center;
  justify-content: center;
  gap: 5px;
  box-shadow: 0 4px 14px rgba(4, 120, 87, 0.5);
  transition: all 0.2s ease;
  letter-spacing: 0.02em;
}

.curved-card .enter-valley-badge i {
  font-size: 0.85rem;
  transition: transform 0.2s ease;
}

/* Positions Along the Smiling Arc */
.curved-card.slot-far-left {
  transform: translate(-300px, 45px) rotate(-18deg) scale(0.82);
  z-index: 2;
  opacity: 0.65;
  filter: brightness(0.75);
}

.curved-card.slot-left {
  transform: translate(-150px, 15px) rotate(-9deg) scale(0.92);
  z-index: 5;
  opacity: 0.85;
  filter: brightness(0.9);
}

.curved-card.slot-center {
  transform: translate(0px, -8px) rotate(0deg) scale(1.18);
  z-index: 15;
  opacity: 1;
  filter: brightness(1.05);
  border: 3px solid #34D399;
  box-shadow: 0 25px 60px rgba(0, 0, 0, 0.8), 0 0 35px rgba(52, 211, 153, 0.45);
}

.curved-card.slot-center .enter-valley-badge {
  display: inline-flex;
  animation: pulseGlow 2.5s infinite;
}

.curved-card.slot-center:hover {
  transform: translate(0px, -15px) rotate(0deg) scale(1.22);
  border-color: #6EE7B7;
  box-shadow: 0 30px 70px rgba(0, 0, 0, 0.9), 0 0 45px rgba(52, 211, 153, 0.7);
}

.curved-card.slot-center:hover .enter-valley-badge {
  background: #059669;
  transform: scale(1.06);
}

.curved-card.slot-center:hover .enter-valley-badge i {
  transform: translateX(3px);
}

@keyframes pulseGlow {
  0%, 100% {
    box-shadow: 0 0 0 0 rgba(52, 211, 153, 0.7);
  }
  50% {
    box-shadow: 0 0 0 10px rgba(52, 211, 153, 0);
  }
}

.curved-card.slot-right {
  transform: translate(150px, 15px) rotate(9deg) scale(0.92);
  z-index: 5;
  opacity: 0.85;
  filter: brightness(0.9);
}

.curved-card.slot-far-right {
  transform: translate(300px, 45px) rotate(18deg) scale(0.82);
  z-index: 2;
  opacity: 0.65;
  filter: brightness(0.75);
}

.curved-card.slot-hidden {
  transform: translate(0, 100px) scale(0.5);
  opacity: 0;
  pointer-events: none;
}

/* ==========================================================================
   CARDS & CONTAINERS (High-Contrast Clean White Surfaces)
   ========================================================================== */
.clean-white-card,
.deosai-card,
.tour-catalog-card {
  background: #FFFFFF !important;
  border: 1px solid var(--border-light) !important;
  border-radius: 20px !important;
  box-shadow: var(--shadow-sm);
  transition: var(--transition-smooth);
  overflow: hidden;
}

.clean-white-card:hover,
.deosai-card:hover,
.tour-catalog-card:hover {
  transform: translateY(-5px);
  box-shadow: var(--shadow-md);
  border-color: var(--border-medium) !important;
}

.package-card-img-wrap,
.tour-img-wrapper {
  position: relative;
  height: 220px;
  overflow: hidden;
}

.package-card-img-wrap img,
.tour-card-img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.6s ease;
}

.badge-tag-amber,
.tour-badge-pill {
  position: absolute;
  top: 14px;
  left: 14px;
  background: #FFFBEB !important;
  color: #B45309 !important;
  border: 1px solid #FDE68A !important;
  font-family: var(--font-mono);
  font-weight: 700;
  font-size: 0.75rem;
  padding: 4px 10px;
  border-radius: 6px;
  z-index: 2;
}

/* ==========================================================================
   INNER PAGE HEADERS (Distinctive Themed Banners with White Headers)
   ========================================================================== */
.inner-page-header {
  position: relative;
  padding: 70px 0 45px 0;
  background: linear-gradient(135deg, #064E3B 0%, #022C22 100%);
  color: #FFFFFF !important;
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

.inner-page-header h1 {
  color: #FFFFFF !important;
}

.inner-page-header p {
  color: rgba(255, 255, 255, 0.9) !important;
}

.breadcrumb-custom {
  font-size: 0.85rem;
}

.breadcrumb-custom a {
  color: #A7F3D0 !important;
  text-decoration: none;
}

.breadcrumb-custom .active {
  color: rgba(255, 255, 255, 0.75) !important;
}

/* ==========================================================================
   UNIQUE VALLEY THEME ACCENTS FOR DESTINATION PAGES
   ========================================================================== */
/* Hunza Page Accent: Apricot Gold & Turquoise */
body.theme-hunza .inner-page-header {
  background: linear-gradient(135deg, #78350F 0%, #064E3B 100%) !important;
}
body.theme-hunza .btn-pine {
  background: #B45309 !important;
}
body.theme-hunza .btn-pine:hover {
  background: #92400E !important;
}

/* Skardu & Deosai Page Accent: Deep Sapphire & Sand Dune */
body.theme-skardu .inner-page-header {
  background: linear-gradient(135deg, #1E3A8A 0%, #064E3B 100%) !important;
}
body.theme-skardu .btn-pine {
  background: #1E3A8A !important;
}
body.theme-skardu .btn-pine:hover {
  background: #172554 !important;
}

/* Fairy Meadows Page Accent: Alpine Fir & Nanga Glacier */
body.theme-fairymeadows .inner-page-header {
  background: linear-gradient(135deg, #14532D 0%, #0F172A 100%) !important;
}
body.theme-fairymeadows .btn-pine {
  background: #14532D !important;
}
body.theme-fairymeadows .btn-pine:hover {
  background: #052E16 !important;
}

/* Swat Valley Page Accent: Emerald Meadow */
body.theme-swat .inner-page-header {
  background: linear-gradient(135deg, #047857 0%, #064E3B 100%) !important;
}
body.theme-swat .btn-pine {
  background: #047857 !important;
}
body.theme-swat .btn-pine:hover {
  background: #064E3B !important;
}

/* K2 Trekking Accent: Extreme Mountain Crimson */
body.theme-k2 .inner-page-header {
  background: linear-gradient(135deg, #991B1B 0%, #0F172A 100%) !important;
}
body.theme-k2 .btn-pine {
  background: #991B1B !important;
}
body.theme-k2 .btn-pine:hover {
  background: #7F1D1D !important;
}

/* Valley Telemetry Strip */
.telemetry-bar {
  background: #FFFFFF;
  border: 1px solid var(--border-light);
  border-radius: 18px;
  padding: 16px 24px;
  box-shadow: var(--shadow-sm);
  margin-top: -30px;
  position: relative;
  z-index: 10;
}
.telemetry-item {
  display: flex;
  align-items: center;
  gap: 12px;
}
.telemetry-icon {
  width: 44px;
  height: 44px;
  border-radius: 12px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.25rem;
}
body.theme-skardu .telemetry-icon { background: rgba(30, 58, 138, 0.1); color: #1E3A8A; }
body.theme-hunza .telemetry-icon { background: rgba(217, 119, 6, 0.12); color: #D97706; }
body.theme-fairymeadows .telemetry-icon { background: rgba(20, 83, 45, 0.1); color: #14532D; }
body.theme-swat .telemetry-icon { background: rgba(4, 120, 87, 0.1); color: #047857; }
body.theme-k2 .telemetry-icon { background: rgba(153, 27, 27, 0.1); color: #991B1B; }

/* ==========================================================================
   CALCULATOR CARD (Clean High-Contrast)
   ========================================================================== */
.calculator-clean-card {
  background: #FFFFFF !important;
  border: 1px solid var(--border-medium) !important;
  border-radius: 24px;
  box-shadow: var(--shadow-md);
  padding: 2.5rem;
}

.output-price-box {
  background: #064E3B !important;
  color: #FFFFFF !important;
  border-radius: 20px;
  padding: 2.2rem;
  text-align: center;
}

.output-price-box .price-huge {
  font-family: var(--font-mono);
  font-size: clamp(2.4rem, 4vw, 3.4rem);
  font-weight: 800;
  color: #FFFFFF !important;
  margin: 0.5rem 0;
}

.output-price-box .price-huge span {
  color: #34D399 !important;
}

.clean-pill-option {
  background: #F8FAFC !important;
  border: 1px solid var(--border-medium) !important;
  color: var(--text-main) !important;
  font-weight: 600;
  font-size: 0.88rem;
  padding: 0.75rem 1rem;
  border-radius: 12px;
  cursor: pointer;
  width: 100%;
  text-align: center;
  transition: var(--transition-fast);
}

.clean-pill-option.active,
.clean-pill-option:hover {
  background: #ECFDF5 !important;
  border-color: #047857 !important;
  color: #047857 !important;
}

/* ==========================================================================
   ACCORDIONS (Itinerary Timelines & FAQs - High Contrast)
   ========================================================================== */
.itinerary-accordion .accordion-item {
  background: #FFFFFF !important;
  border: 1px solid var(--border-light) !important;
  border-radius: 14px !important;
  margin-bottom: 12px;
  overflow: hidden;
  box-shadow: var(--shadow-sm);
}

.itinerary-accordion .accordion-button {
  background: #FFFFFF !important;
  color: #0F172A !important;
  font-weight: 700;
  font-size: 1rem;
  padding: 1.2rem;
  box-shadow: none !important;
}

.itinerary-accordion .accordion-button:not(.collapsed) {
  background: #ECFDF5 !important;
  color: #047857 !important;
  border-bottom: 1px solid #D1FAE5 !important;
}

.itinerary-accordion .accordion-body {
  color: #334155 !important;
  font-size: 0.95rem;
  padding: 1.4rem;
  line-height: 1.7;
}

/* Checklist Items */
.checklist-item {
  background: #F8FAFC !important;
  border: 1px solid var(--border-light) !important;
  border-radius: 12px;
  padding: 1rem 1.2rem;
  margin-bottom: 10px;
  display: flex;
  align-items: center;
  gap: 14px;
  cursor: pointer;
  color: #0F172A !important;
  font-weight: 600;
  transition: var(--transition-fast);
}

.checklist-item:hover {
  background: #ECFDF5 !important;
  border-color: #A7F3D0 !important;
}

.checklist-item.checked {
  background: #F0FDF4 !important;
  border-color: #34D399 !important;
}

.checklist-item.checked span {
  text-decoration: line-through;
  color: #94A3B8 !important;
}

/* ==========================================================================
   FOOTER (High-Contrast Slate)
   ========================================================================== */
.footer-clean,
.footer-deosai {
  background: #0F172A !important;
  color: #94A3B8 !important;
  padding: 70px 0 30px 0;
  font-size: 0.92rem;
}

.footer-clean h5, .footer-clean h6,
.footer-deosai h5, .footer-deosai h6,
.footer-heading {
  color: #FFFFFF !important;
  font-weight: 700;
}

.footer-clean a,
.footer-deosai a,
.footer-link {
  color: #CBD5E1 !important;
  text-decoration: none;
  display: block;
  margin-bottom: 0.6rem;
  transition: color 0.2s;
}

.footer-clean a:hover,
.footer-deosai a:hover,
.footer-link:hover {
  color: #34D399 !important;
}

/* Floating WhatsApp Button */
.whatsapp-floating-clean,
.whatsapp-btn-float {
  position: fixed;
  bottom: 25px;
  right: 25px;
  width: 58px;
  height: 58px;
  border-radius: 50%;
  background: #25D366 !important;
  color: #FFFFFF !important;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.8rem;
  box-shadow: 0 10px 25px rgba(37, 211, 102, 0.4);
  z-index: 1000;
  text-decoration: none;
  transition: transform 0.3s ease;
}

.whatsapp-floating-clean:hover,
.whatsapp-btn-float:hover {
  transform: scale(1.1);
  color: #FFFFFF !important;
}

/* Mobile Responsive */
@media (max-width: 991px) {
  .arched-carousel-wrapper {
    height: 220px;
  }
  .curved-card {
    width: 130px;
    height: 180px;
  }
  .curved-card.slot-far-left {
    transform: translate(-190px, 30px) rotate(-15deg) scale(0.75);
  }
  .curved-card.slot-left {
    transform: translate(-95px, 10px) rotate(-8deg) scale(0.85);
  }
  .curved-card.slot-center {
    transform: translate(0px, 0px) rotate(0deg) scale(1.05);
  }
  .curved-card.slot-right {
    transform: translate(95px, 10px) rotate(8deg) scale(0.85);
  }
  .curved-card.slot-far-right {
    transform: translate(190px, 30px) rotate(15deg) scale(0.75);
  }
}
```

---

## Assistant (2026-11-28T08:30:55Z)

Running live browser QA verification on `pages/tips.html` across desktop and mobile viewports.

---

## Assistant (2026-11-28T08:34:07Z)

Verifying the updated footer contrast and spacing in the browser.

---

## Assistant (2026-11-28T08:34:42Z)

I have created the **Travel Tips & Safety** page for **DEOSAI Expeditions** using your shared `css/style.css` and `js/main.js` classes and IDs, without creating any of the remaining pages.

> **Workspace recommendation:** Since no workspace was active, I set up the project subdirectory at `C:\Users\HAROON TRADERS\.gemini\antigravity\scratch\deosai-expeditions`. Please set that folder as your active workspace when continuing work on the remaining pages.

### Files Created
- [pages/tips.html](file:///C:/Users/HAROON%20TRADERS/.gemini/antigravity/scratch/deosai-expeditions/pages/tips.html) — The responsive Travel Tips & Safety page.
- [css/style.css](file:///C:/Users/HAROON%20TRADERS/.gemini/antigravity/scratch/deosai-expeditions/css/style.css) — Stored verbatim from your shared stylesheet so `../css/style.css` resolves cleanly.
- [js/main.js](file:///C:/Users/HAROON%20TRADERS/.gemini/antigravity/scratch/deosai-expeditions/js/main.js) — Stored verbatim from your shared interactive script so `../js/main.js` resolves cleanly.

### Page Implementation Summary
1. **Top Contact & Safety Information Strip** (`.top-contact-strip`): Displays DTS License `#PK-8842`, 24/7 Field Safety Dispatch, medical O₂ & satellite support, and clickable phone link `+92 (300) 000-0000` (`d-none d-md-block`).
2. **Responsive Main Navigation Bar** (`.navbar-alpine`): Uses `.brand-wrapper`, `.brand-title-alpine`, `.brand-sub-alpine`, `.nav-link-alpine` (with `active` on `Travel Tips`), `Destinations` and `Tour Packages` Bootstrap dropdowns, the `#curr-pkr` / `#curr-usd` currency switcher inside `.curr-switch-box` (matching `initCurrencySwitcher()` in `js/main.js`), and the `.btn-pine` `Plan Trip →` CTA.
3. **Travel Tips & Safety Hero Section** (`.inner-page-header`): Includes `.breadcrumb-custom`, a legible `bg-white bg-opacity-25` `FIELD ESSENTIALS & SAFETY` badge, main heading, and lead description.
4. **Six Travel Advisory Information Cards** (`.clean-white-card` + `.text-pine` Bootstrap Icons in a responsive `col-lg-4 col-md-6` grid):
   - Pakistan Online e-Visa (`bi-passport`)
   - NOC & Restricted Areas (`bi-file-earmark-check`)
   - SCOM SIM Card (Telecom) (`bi-broadcast-pin`)
   - Currency & ATMs (`bi-cash-stack`)
   - Altitude Health (AMS) (`bi-heart-pulse`)
   - Packing & Dress Etiquette (`bi-backpack2`)
5. **Safety & Logistics FAQs** (`.itinerary-accordion`, `#faqAccordion`): Bootstrap 5.3.3 accordion with three questions (`#faq1` expanded initially, `#faq2` and `#faq3` collapsed with `data-bs-parent="#faqAccordion"`).
6. **Consistent Website Footer** (`.footer-clean`): Three-column layout with `text-white-50` contrast on the dark slate footer background and bottom/right spacing (`pb-5` / `pe-lg-5`) so `"Ask Our Operations Desk →"` stays clear of the floating button.
7. **Floating WhatsApp Contact Button** (`.whatsapp-floating-clean`): Fixed bottom-right WhatsApp button linking to `https://wa.me/923000000000` with `rel="noopener noreferrer"` and `aria-label="Chat on WhatsApp"`.

### Verification & Testing Performed
- **Static HTML & Asset Validation (`check_tips.py`)**: Verified after the final edit that `../css/style.css` and `../js/main.js` exist relative to `pages/tips.html`, all required IDs (`curr-pkr`, `curr-usd`, `faqAccordion`, `faq1`, `faq2`, `faq3`, `navGuide`) and stylesheet classes are present, and HTML tags are balanced with zero unclosed or mismatched tags.
- **Browser QA (`http://localhost:8765/pages/tips.html`)**:
  - Verified HTTP `200` loading of `pages/tips.html`, `css/style.css`, and `js/main.js` with zero console errors.
  - Verified desktop (`1440x900`) and mobile (`375x812`) layouts render with no horizontal overflow, `.top-contact-strip` hides on mobile, and `.navbar-toggler` collapses/expands the mobile nav menu.
  - Tested `Destinations` and `Tour Packages` dropdowns, `#faqAccordion` expand/collapse transitions across `#faq1`–`#faq3`, and `#curr-usd` / `#curr-pkr` currency pill toggling.
  - Caught and fixed two footer issues from the initial browser pass: updated the `FIELD ESSENTIALS & SAFETY` badge to `bg-white bg-opacity-25` (valid in Bootstrap 5.3.3), added `text-white-50` for footer contrast against `.footer-clean`, and added bottom/right clearance so `.whatsapp-floating-clean` does not overlap `"Ask Our Operations Desk →"` (re-verified on the final screenshot at `1440x900` with zero overlap).
  - *Note:* Internal links (`../index.html`, `contact.html`, `planner.html`, and the other destination/section `.html` pages) were verified for correct relative paths, though their target files are not yet created per your scope.

---

## User (2026-11-28T08:44:52Z)

export this chat as "session-01.md"
include every command that i gave and your respone

---
