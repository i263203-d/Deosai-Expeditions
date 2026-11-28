# Session 01 — DEOSAI Expeditions (Travel Tips & Safety Page)

- **Conversation ID:** `cd531357-fa2a-4237-8674-3e52464aafff`
- **Date:** 2026-11-28

---

## User (2026-11-28T08:11:14Z)
# Project Task: Develop the Contact Us Page – DEOSAI Expeditions

I am working on a university IICT website project called DEOSAI Expeditions. My task is to develop a professional, visually attractive and fully responsive Contact Us page as an integral part of the existing website.

The objective is to provide visitors with an easy way to contact DEOSAI Expeditions, ask questions about tours, request travel information and submit enquiries.

## 1. Understand the Existing Project

Before starting development:

- Inspect the complete project folder and understand its directory structure.
- Examine the homepage and other available HTML pages.
- Study the existing `css/style.css` and `js/main.js` files.
- Understand the website's branding, typography, color palette and layout.
- Examine how the existing navbar, footer, buttons, cards and responsive layouts are implemented.
- Identify existing reusable components and CSS classes.
- Check existing contact information and links so that the same details are used consistently.

Do not modify unrelated pages or shared functionality unnecessarily.

## 2. Main Objective

Develop a dedicated `contact.html` page for DEOSAI Expeditions.

The page should provide a professional contact experience while maintaining the same visual identity as the rest of the website.

Use a clean alpine tourism aesthetic with pine-green colors, natural tones, professional typography, subtle shadows and well-organized layouts.

## 3. Required Page Structure

### A. Top Contact and Safety Strip

Include the same top information strip used across the website.

Display:
- Government of Pakistan DTS License information.
- 24/7 Field Safety Dispatch.
- Medical O₂ & Satellite Support.
- Existing contact telephone number.

Maintain consistency with other pages.

### B. Main Navigation Bar

Use the existing DEOSAI navigation structure.

Include:
- DEOSAI EXPEDITIONS logo.
- Home.
- Destinations dropdown.
- Tour Packages dropdown.
- Gallery.
- Reviews.
- Travel Tips.
- Blog.
- Contact (active navigation item).
- PKR/USD currency switch.
- Plan Trip button.

Ensure all links use the correct existing page paths.

The navbar must be responsive and fully functional.

### C. Contact Page Hero Section

Create an attractive inner-page header.

Include:
- Breadcrumb: Home / Contact.
- Small badge: GET IN TOUCH.
- Main heading: Contact Us.
- Supporting description:

"Have questions about your next adventure in Northern Pakistan? Our team is here to help you plan your journey, answer your questions and make your expedition memorable."

Use the existing inner-page header design and typography.

### D. Contact Information Section

Create an organized and visually appealing contact information area.

Include separate information cards for:

**1. Call Us**

Display the existing website telephone number.

Provide a clickable telephone link using `tel:`.

**2. Email Us**

Display the existing official website email address, if available.

Provide a clickable `mailto:` link.

**3. WhatsApp**

Provide a WhatsApp contact option using the existing website contact number.

**4. Our Location**

Display the existing company office or location information if it is available in the project.

Do not invent telephone numbers, email addresses, office addresses or business details. Reuse existing project information.

Use appropriate Bootstrap Icons and consistent styling.

### E. Contact Enquiry Form

Create a professional contact form with the following fields:

1. Full Name (required).
2. Email Address (required).
3. Phone / WhatsApp Number.
4. Subject (required).
5. Enquiry Type (dropdown):
   - General Enquiry.
   - Tour Packages.
   - Custom Trip Planning.
   - Destinations Information.
   - Travel Assistance.
   - Other.
6. Message (required).

Include a clear Submit Message button.

Form design requirements:

- Proper labels for every field.
- Appropriate input types.
- Required-field validation.
- Clear spacing and alignment.
- Responsive layout.
- Consistent input borders and focus states.
- User-friendly error messages.

If the project does not have a backend, implement appropriate client-side validation and a clear success message without falsely claiming that an enquiry has been delivered to the company.

Do not introduce unnecessary backend dependencies.

### F. Additional Assistance Section

Create a visually attractive section encouraging visitors to contact the team for travel planning and assistance.

Suggested heading:

"Let's Plan Your Next Adventure"

Supporting text:

"Whether you are exploring Hunza, discovering Skardu or preparing for a Northern Pakistan expedition, our team is ready to help you get started."

Include a Plan Your Trip button linking to the existing `planner.html` page.

Maintain the existing website's button styling.

### G. Location / Map Section

If an actual company location is available in the project, include a location section with an embedded map or location link.

Use the correct verified address.

If no verified address is available, do not invent one. Keep the location section simple or omit the map.

Ensure the map does not affect mobile responsiveness.

### H. Footer

Use the same footer structure and appearance as the existing website.

Include:
- DEOSAI EXPEDITIONS branding.
- Existing DTS license information.
- Copyright 2026 DEOSAI Expeditions (Pvt) Ltd.
- Relevant contact links.

### I. Floating WhatsApp Button

Include the existing floating WhatsApp contact button.

Use the same appearance, icon and positioning as the other website pages.

## 4. Technical Requirements

- Use HTML5.
- Use Bootstrap 5.3.3.
- Use Bootstrap Icons 1.11.3.
- Use existing Google Fonts.
- Connect the existing shared `css/style.css`.
- Connect the existing shared `js/main.js`.
- Use correct relative paths.
- Reuse existing CSS classes and components.
- Avoid unnecessary external libraries.
- Avoid duplicate JavaScript functionality.
- Avoid global CSS changes that could affect other pages.
- Do not overwrite unrelated website files.
- Use page-specific CSS classes when additional styling is necessary.

## 5. Design Expectations

The Contact Us page must maintain the DEOSAI Expeditions visual identity.

Design characteristics:

- Professional alpine tourism appearance.
- Pine-green and natural color palette.
- Clean white information cards.
- Consistent typography.
- Subtle shadows.
- Rounded corners.
- Well-spaced form elements.
- Clear headings and section hierarchy.
- Professional icons.
- Responsive Bootstrap layouts.

The page should look consistent with the homepage, Travel Tips, Destinations and Tour Packages sections.

Avoid unnecessary animations, excessive colors or unrelated design elements.

## 6. Responsive Design

Ensure the page works properly on:

- Desktop computers.
- Tablets.
- Mobile phones.

The contact form, information cards, navigation and map must adapt properly to different screen sizes.

Prevent horizontal scrolling and overlapping elements.

## 7. Testing and Verification

After implementation:

- Check all internal navigation links.
- Verify telephone and email links.
- Test all contact form fields.
- Test required-field validation.
- Test the success message.
- Verify navbar dropdowns.
- Check mobile navigation.
- Verify the currency switch remains compatible.
- Check CSS and JavaScript loading.
- Confirm that the footer and WhatsApp button display correctly.
- Verify that other website pages remain unaffected.

If browser preview is available, inspect the completed page at different screen sizes.

## 8. Final Completion

After completing the task:

1. Identify the files created or modified.
2. Explain how the page uses the existing shared CSS and JavaScript.
3. Report any compatibility issues.
4. Summarize the functionality implemented.
5. Confirm the testing performed.
6. Provide the final location of `contact.html`.

Keep the code organized, understandable and appropriate for an introductory university IICT project.

The final Contact Us page should provide a smooth, professional and consistent experience for visitors to DEOSAI Expeditions.
This the page two
Follow the erliear instructions

  <link rel="stylesheet" href="../css/style.css">

  <!-- Page-specific styles for Contact Us (scoped to avoid affecting shared pages) -->
  <style>
    .contact-card-icon {
      width: 48px;
      height: 48px;
      border-radius: 14px;
      background: rgba(4, 120, 87, 0.1);
      color: var(--color-primary);
      display: inline-flex;
      align-items: center;
      justify-content: center;
      font-size: 1.35rem;
      margin-bottom: 1rem;
    }

    .contact-card-icon.whatsapp-accent {
      background: rgba(37, 211, 102, 0.12);
      color: #15803D;
    }

    .contact-info-link {
      color: var(--color-primary);
      font-weight: 600;
      text-decoration: none;
      word-break: break-word;
      transition: var(--transition-fast);
    }

    .contact-info-link:hover {
      color: var(--color-primary-hover);
      text-decoration: underline;
    }

    .contact-form-card { background: var(--bg-surface);
      border: 1px solid var(--border-light);
      border-radius: 24px;
      box-shadow: var(--shadow-md);
    }

    .contact-input {
      border: 1.5px solid var(--border-medium);
      border-radius: 12px;
      padding: 0.7rem 0.95rem;
      font-size: 0.95rem;
      color: var(--text-main);
      background-color: #FFFFFF;
      transition: var(--transition-fast);
    }

    .contact-input:focus {
      border-color: var(--color-primary);
      box-shadow: 0 0 0 0.22rem rgba(4, 120, 87, 0.15);
    }

    .contact-required-mark {
      color: #DC2626 !important;
    }

    #selected-tour-banner:not(.d-none) {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: 1rem;
    }

    .contact-assistance-card {
      background: linear-gradient(135deg, #FFFFFF 0%, #ECFDF5 100%);
      border: 1px solid rgba(4, 120, 87, 0.2);
      border-radius: 24px;
      box-shadow: var(--shadow-md);
    }

    .contact-map-frame {
      border: 0;
      width: 100%;
      height: 100%;
      display: block;
    }

    .curr-switch-box {
      flex-shrink: 0;
    }
     .curr-pill-btn,
    .navbar .btn-pine {
      white-space: nowrap;
    }
  </style>
</head>
<body>

  <!-- 1. Top Contact & Safety Information Strip -->
  <div class="top-contact-strip d-none d-md-block">
    <div class="container d-flex justify-content-between align-items-center">
      <div>
        <i class="bi bi-shield-check text-success me-1"></i> Govt. of Pakistan DTS License #PK-8842 &bull; 24/7 Field Safety Dispatch
      </div>
      <div class="d-flex align-items-center gap-3">
        <span><i class="bi bi-heart-pulse text-warning me-1"></i> Medical O&#8322; &amp; Satellite Support</span>
        <a href="tel:+923000000000"><i class="bi bi-telephone text-success me-1"></i> +92 (300) 000-0000</a>
      </div>
    </div>
  </div>

  <!-- 2. Responsive Main Navigation Bar -->
  <nav class="navbar navbar-expand-lg navbar-light navbar-alpine sticky-top">
    <div class="container">
      <a class="brand-wrapper" href="../index.html">
        <svg width="36" height="36" viewBox="0 0 36 36" fill="none" aria-hidden="true">
          <path d="M5 6C5 4.89543 5.89543 4 7 4H18C25.732 4 32 10.268 32 18C32 25.732 25.732 32 18 32H7C5.89543 32 5 31.1046 5 30V6Z" stroke="#047857" stroke-width="2.5" fill="rgba(4, 120, 87, 0.08)"/>
          <path d="M10 27L17 14L24 27" stroke="#059669" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/>
          <circle cx="17" cy="10" r="2.2" fill="#D97706"/>
        </svg>
        <div>
          <span class="brand-title-alpine">DEOSAI</span>
          <span class="brand-sub-alpine">EXPEDITIONS</span>
        </div>
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navContact" aria-controls="navContact" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navContact">
        <ul class="navbar-nav mx-auto mb-2 mb-lg-0">
          <li class="nav-item"><a class="nav-link nav-link-alpine" href="../index.html">Home</a></li>
          <li class="nav-item dropdown">
            <a class="nav-link nav-link-alpine dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">Destinations</a>
            <ul class="dropdown-menu shadow-lg border-0 rounded-3">
              <li><a class="dropdown-item py-2" href="destinations.html"><i class="bi bi-map text-success me-2"></i>Destinations Overview</a></li>
              <li><hr class="dropdown-divider"></li>
              <li><a class="dropdown-item py-2" href="hunza.html"><i class="bi bi-pin-map text-primary me-2"></i>Hunza Valley</a></li>
              <li><a class="dropdown-item py-2" href="skardu.html"><i class="bi bi-pin-map text-primary me-2"></i>Skardu &amp; Baltistan</a></li>
              <li><a class="dropdown-item py-2" href="swat.html"><i class="bi bi-pin-map text-primary me-2"></i>Swat &amp; Kalam</a></li>
              <li><a class="dropdown-item py-2" href="fairy-meadows.html"><i class="bi bi-pin-map text-primary me-2"></i>Fairy Meadows &amp; Nanga Parbat</a></li>
              <li><a class="dropdown-item py-2" href="chitral.html"><i class="bi bi-pin-map text-primary me-2"></i>Chitral &amp; Kalash</a></li>
            </ul>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link nav-link-alpine dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">Tour Packages</a>
            <ul class="dropdown-menu shadow-lg border-0 rounded-3">
              <li><a class="dropdown-item py-2" href="packages.html"><i class="bi bi-grid text-success me-2"></i>Tour Packages</a></li>
              <li><a class="dropdown-item py-2" href="planner.html"><i class="bi bi-sliders text-info me-2"></i>Custom Trip Planner</a></li>
              <li><a class="dropdown-item py-2" href="seasonal.html"><i class="bi bi-flower1 text-warning me-2"></i>Seasonal Guide</a></li>
            </ul>
          </li>
          <li class="nav-item"><a class="nav-link nav-link-alpine" href="gallery.html">Gallery</a></li>
          <li class="nav-item"><a class="nav-link nav-link-alpine" href="reviews.html">Reviews</a></li>
          <li class="nav-item"><a class="nav-link nav-link-alpine" href="tips.html">Travel Tips</a></li>
          <li class="nav-item"><a class="nav-link nav-link-alpine" href="blog.html">Blog</a></li>
          <li class="nav-item"><a class="nav-link nav-link-alpine active" aria-current="page" href="contact.html">Contact</a></li>
        </ul>
  <div class="d-flex align-items-center gap-3">
          <div class="curr-switch-box">
            <button type="button" class="curr-pill-btn active" id="curr-pkr">&#8360; PKR</button>
            <button type="button" class="curr-pill-btn" id="curr-usd">$ USD</button>
          </div>
          <a href="planner.html" class="btn btn-pine d-none d-sm-inline-flex">Plan Trip &rarr;</a>
        </div>
      </div>
    </div>
  </nav>

  <!-- 3. Contact Page Hero Section -->
  <header class="inner-page-header">
    <div class="container position-relative z-2">
      <nav aria-label="breadcrumb">
        <ol class="breadcrumb breadcrumb-custom mb-2">
          <li class="breadcrumb-item"><a href="../index.html">Home</a></li>
          <li class="breadcrumb-item active" aria-current="page">Contact</li>
        </ol>
      </nav>
      <span class="badge bg-white bg-opacity-25 text-white font-mono small px-3 py-1 mb-2">
        <i class="bi bi-chat-dots text-warning me-1"></i> GET IN TOUCH
      </span>
      <h1 class="display-4 fw-bold text-white mt-1">Contact Us</h1>
      <p class="lead text-light mb-0" style="max-width: 680px;">
        Have questions about your next adventure in Northern Pakistan? Our team is here to help you plan your journey, answer your questions and make your expedition memorable.
      </p>
    </div>
  </header>
        <div id="selected-tour-banner" class="alert alert-success d-none rounded-4 p-4 mb-5 shadow-sm" role="alert">
        <div>
          <span class="font-mono small fw-bold text-uppercase d-block text-pine">// SELECTED FOR ENQUIRY</span>
          <strong class="fs-5" id="selected-tour-name">Tour Package</strong>
        </div>
        <span class="badge bg-success px-3 py-2 font-mono">Pre-filled Below</span>
      </div>

      <!-- Contact Information Cards -->
      <div class="text-center mb-4">
        <span class="font-mono text-pine small fw-bold">// DIRECT CHANNELS</span>
        <h2 class="display-6 fw-bold mt-1">Reach Our Expedition Desk</h2>
      </div>

      <div class="row g-4 mb-5">
        <!-- 1. Call Us -->
        <div class="col-md-6 col-xl-3">
          <div class="clean-white-card h-100 p-4">
            <div class="contact-card-icon">
              <i class="bi bi-telephone-outbound"></i>
            </div>
            <h4 class="fw-bold mb-2">Call Us</h4>
            <p class="text-muted small mb-3">
              Speak directly with our 24/7 field safety and dispatch team for urgent travel support.
            </p>
            <div class="d-flex flex-column gap-1 small">
              <a href="tel:+923000000000" class="contact-info-link">
                <i class="bi bi-telephone me-1"></i> +92 (300) 000-0000
              </a>
              <a href="tel:+92518809900" class="contact-info-link text-muted fw-medium">
                Islamabad: +92 (51) 880-9900
              </a>
              <a href="tel:+925815450200" class="contact-info-link text-muted fw-medium">
                Skardu: +92 (5815) 450-200
              </a>
            </div>
          </div>
        </div>

        <!-- 2. Email Us -->
        <div class="col-md-6 col-xl-3">
          <div class="clean-white-card h-100 p-4">
            <div class="contact-card-icon">
              <i class="bi bi-envelope-at"></i>
            </div>
  <h4 class="fw-bold mb-2">Email Us</h4>
            <p class="text-muted small mb-3">
              Send itinerary requests, visa LOI documentation queries, or custom group proposals.
            </p>
            <a href="mailto:islamabad@deosai.pk" class="contact-info-link small d-inline-flex align-items-center gap-1">
              <i class="bi bi-envelope"></i> islamabad@deosai.pk
            </a>
          </div>
        </div>

        <!-- 3. WhatsApp -->
        <div class="col-md-6 col-xl-3">
          <div class="clean-white-card h-100 p-4">
            <div class="contact-card-icon whatsapp-accent">
              <i class="bi bi-whatsapp"></i>
            </div>
            <h4 class="fw-bold mb-2">WhatsApp</h4>
            <p class="text-muted small mb-3">
              Message our operations desk on WhatsApp for quick responses, route checks, and quotes.
            </p>
            <a id="whatsapp-booking-btn" href="https://wa.me/923000000000?text=Salam%20DEOSAI%20Expeditions!%20I%20have%20an%20enquiry." target="_blank" rel="noopener noreferrer" class="contact-info-link small d-inline-flex align-items-center gap-1">
              <i class="bi bi-whatsapp"></i> +92 (300) 000-0000 &rarr;
            </a>
          </div>
        </div>

        <!-- 4. Our Location -->
        <div class="col-md-6 col-xl-3">
          <div class="clean-white-card h-100 p-4">
            <div class="contact-card-icon">
              <i class="bi bi-geo-alt"></i>
            </div>
            <h4 class="fw-bold mb-2">Our Location</h4>
            <p class="text-muted small mb-2">
              <strong class="text-dark">Islamabad HQ:</strong> Plot 44, Blue Area, Jinnah Avenue, Islamabad, Pakistan
            </p>
            <p class="text-muted small mb-0">
              <strong class="text-dark">Skardu Base:</strong> Main Airport Road, Near Serena Shigar Junction, Skardu
            </p>
          </div>
        </div>
      </div>
 <!-- Contact Enquiry Form -->
      <div class="row justify-content-center" id="contact-form-section">
        <div class="col-lg-10 col-xl-9">
          <div class="contact-form-card p-4 p-md-5">
            <div class="mb-4">
              <span class="font-mono text-pine small fw-bold">// SEND AN ENQUIRY</span>
              <h2 class="h3 fw-bold mt-1 mb-2">Submit Your Message</h2>
              <p class="text-muted small mb-0">
                Complete the form below with your travel questions or tour preferences. Fields marked with <span class="contact-required-mark fw-bold">*</span> are required.
              </p>
            </div>

            <div id="form-error-summary" class="alert alert-danger d-none rounded-3 small mb-4" role="alert">
              <i class="bi bi-exclamation-triangle-fill me-2"></i>
              Please review and correct the highlighted fields below before submitting.
            </div>

            <form id="booking-inquiry-form" novalidate>
              <div class="row g-3">
                <!-- 1. Full Name (required) -->
                <div class="col-md-6">
                  <label for="booking-name" class="form-label small fw-bold">
                    Full Name <span class="contact-required-mark">*</span>
                  </label>
                  <input type="text" id="booking-name" name="fullName" class="form-control contact-input" placeholder="e.g. Ayesha Siddiqui" required>
                  <div class="invalid-feedback">Please enter your full name.</div>
                </div>

                <!-- 2. Email Address (required) -->
                <div class="col-md-6">
                  <label for="booking-email" class="form-label small fw-bold">
                    Email Address <span class="contact-required-mark">*</span>
                  </label>
                  <input type="email" id="booking-email" name="email" class="form-control contact-input" placeholder="name@example.com" required>
                  <div class="invalid-feedback">Please enter a valid email address.</div>
                </div>
                <!-- 3. Phone / WhatsApp Number (optional) -->
                <div class="col-md-6">
                  <label for="booking-phone" class="form-label small fw-bold">
                    Phone / WhatsApp Number <span class="text-muted fw-normal">(Optional)</span>
                  </label>
                  <input type="tel" id="booking-phone" name="phone" class="form-control contact-input" placeholder="+92 300 0000000">
                  <div class="invalid-feedback">Please enter a valid phone number (at least 7 digits) or leave this blank.</div>
                </div>

                <!-- 5. Enquiry Type (dropdown) -->
                <div class="col-md-6">
                  <label for="booking-subject" class="form-label small fw-bold">
                    Enquiry Type <span class="contact-required-mark">*</span>
                  </label>
                  <select id="booking-subject" name="enquiryType" class="form-select contact-input" required>
                    <option value="General Enquiry" selected>General Enquiry</option>
                    <option value="Tour Packages">Tour Packages</option>
                    <option value="Custom Trip Planning">Custom Trip Planning</option>
                    <option value="Destinations Information">Destinations Information</option>
                    <option value="Travel Assistance">Travel Assistance</option>
                    <option value="Other">Other</option>
                  </select>
                  <div class="invalid-feedback">Please select an enquiry type.</div>
                </div>

                <!-- 4. Subject (required) -->
                <div class="col-12">
                  <label for="contact-subject" class="form-label small fw-bold">
                    Subject <span class="contact-required-mark">*</span>
                  </label>
                  <input type="text" id="contact-subject" name="subject" class="form-control contact-input" placeholder="Brief topic of your enquiry (e.g. October Hunza &amp; Skardu itinerary)" required>
                  <div class="invalid-feedback">Please enter a subject for your enquiry.</div>
                </div>
                      <span class="small text-muted">
                    <i class="bi bi-info-circle text-pine me-1"></i> Static demo form: validates locally and prepares your message for WhatsApp or Email.
                  </span>
                  <button type="submit" class="btn btn-pine btn-lg px-4">
                    <i class="bi bi-send me-1"></i> Submit Message
                  </button>
                </div>
              </div>
            </form>

            <!-- Client-Side Validation Success Summary (no false delivery claims) -->
            <div id="booking-confirmation" class="alert alert-success d-none mt-4 rounded-4 p-4 mb-0" role="status" aria-live="polite">
              <h5 class="fw-bold mb-2">
                <i class="bi bi-check-circle-fill me-2"></i>Enquiry Prepared Successfully
              </h5>
              <p class="small mb-3">
                Your enquiry details passed validation and are ready below. Because this website runs statically in your browser without a live backend server, this form has <strong>not</strong> been automatically transmitted. Use either button below to send your prepared message directly to our team:
              </p>
              <div class="d-flex flex-wrap gap-2">
                <a id="booking-confirm-wa" href="https://wa.me/923000000000" target="_blank" rel="noopener noreferrer" class="btn btn-pine">
                  <i class="bi bi-whatsapp me-2"></i> Send via WhatsApp &rarr;
                </a>
                <a id="booking-confirm-email" href="mailto:islamabad@deosai.pk" class="btn btn-pine-outline">
                  <i class="bi bi-envelope me-2"></i> Send via Email
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
 </div>
  </section>

  <!-- 5. Additional Assistance Section -->
  <section class="py-5" style="background: var(--bg-subtle);">
    <div class="container py-3">
      <div class="contact-assistance-card p-4 p-md-5">
        <div class="row align-items-center g-4">
          <div class="col-lg-8">
            <span class="font-mono text-pine small fw-bold">// PERSONALIZED TRAVEL ASSISTANCE</span>
            <h2 class="display-6 fw-bold mt-1 mb-3">Let's Plan Your Next Adventure</h2>
            <p class="text-body mb-0">
              Whether you are exploring Hunza, discovering Skardu or preparing for a Northern Pakistan expedition, our team is ready to help you get started.
            </p>
          </div>
          <div class="col-lg-4 text-lg-end">
            <a href="planner.html" class="btn btn-pine btn-lg">
              Plan Your Trip &rarr;
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- 6. Location / Map Section -->
  <section class="py-5" style="background: var(--bg-surface);">
    <div class="container py-3">
      <div class="text-center mb-5">
        <span class="font-mono text-pine small fw-bold">// VERIFIED OFFICES</span>
        <h2 class="display-6 fw-bold mt-1">Find Us in Islamabad &amp; Skardu</h2>
        <p class="text-muted mx-auto mb-0" style="max-width: 620px;">
          Visit our Islamabad Staging Headquarters or coordinate with our Skardu Field Operations Base for Karakoram logistics.
        </p>
      </div>
<div class="row g-4 align-items-stretch">
        <div class="col-lg-5">
          <div class="d-flex flex-column gap-4 h-100">
            <div class="clean-white-card p-4 flex-grow-1">
              <h5 class="fw-bold mb-2">
                <i class="bi bi-building text-pine me-2"></i>Islamabad Staging Headquarters
              </h5>
              <p class="text-muted small mb-2">
                <i class="bi bi-geo-alt text-pine me-1"></i> Plot 44, Blue Area, Jinnah Avenue, Islamabad, Pakistan
              </p>
              <p class="text-muted small mb-2">
                <i class="bi bi-telephone text-pine me-1"></i>
                <a href="tel:+92518809900" class="contact-info-link">+92 (51) 880-9900</a> &bull;
                <a href="tel:+923000000000" class="contact-info-link">+92 (300) 000-0000</a>
              </p>
              <p class="text-muted small mb-3">
                <i class="bi bi-envelope text-pine me-1"></i>
                <a href="mailto:islamabad@deosai.pk" class="contact-info-link">islamabad@deosai.pk</a>
              </p>
              <a href="https://maps.google.com/?q=Blue+Area,+Jinnah+Avenue,+Islamabad,+Pakistan" target="_blank" rel="noopener noreferrer" class="btn btn-sm btn-pine-outline">
                <i class="bi bi-map me-1"></i> View Islamabad on Google Maps
              </a>
            </div>

            <div class="clean-white-card p-4 flex-grow-1">
              <h5 class="fw-bold mb-2">
                <i class="bi bi-compass text-pine me-2"></i>Skardu Field Operations Base
              </h5>
              <p class="text-muted small mb-2">
                <i class="bi bi-geo-alt text-pine me-1"></i> Main Airport Road, Near Serena Shigar Junction, Skardu
              </p>
              <p class="text-muted small mb-2">
                <i class="bi bi-telephone text-pine me-1"></i>
                <a href="tel:+925815450200" class="contact-info-link">+92 (5815) 450-200</a>
              </p>
              <p class="text-muted small mb-3">
                <i class="bi bi-broadcast text-pine me-1"></i> Satellite Emergency Dispatch: Active 24/7
              </p>
              <a href="https://maps.google.com/?q=Main+Airport+Road,+Skardu,+Pakistan" target="_blank" rel="noopener noreferrer" class="btn btn-sm btn-pine-outline">
                <i class="bi bi-map me-1"></i> View Skardu on Google Maps
              </a>
            </div>
          </div>
        </div>

        <div class="col-lg-7">
          <div class="clean-white-card h-100 p-2">
            <div class="ratio ratio-16x9 h-100 rounded-4 overflow-hidden" style="min-height: 320px;">
              <iframe
                title="DEOSAI Expeditions Islamabad Headquarters Map"
                src="https://www.google.com/maps?q=Blue+Area,+Jinnah+Avenue,+Islamabad,+Pakistan&output=embed"
                class="contact-map-frame"
                loading="lazy"
                referrerpolicy="no-referrer-when-downgrade"
                allowfullscreen>
              </iframe>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- 7. Consistent Website Footer -->
  <footer class="footer-clean pb-5">
    <div class="container pb-3 text-center text-md-start">
      <div class="row g-4 align-items-center">
        <div class="col-lg-4">
          <h5 class="text-white fw-bold font-mono">DEOSAI <span class="text-success">EXPEDITIONS</span></h5>
          <p class="small text-white-50 mb-0">Licensed by the Department of Tourist Services, Government of Pakistan (Lic #PK-8842).</p>
        </div>
        <div class="col-lg-4 text-center">
          <span class="small text-white-50">&copy; 2026 DEOSAI Expeditions (Pvt) Ltd. All rights reserved.</span>
        </div>
        <div class="col-lg-4 text-md-end pe-lg-5">
          <div class="d-flex flex-wrap justify-content-center justify-content-md-end gap-3">
            <a href="tel:+923000000000" class="text-success text-decoration-none small mb-0 d-inline-block"><i class="bi bi-telephone me-1"></i> +92 (300) 000-0000</a>
            <a href="mailto:islamabad@deosai.pk" class="text-success text-decoration-none small mb-0 d-inline-block"><i class="bi bi-envelope me-1"></i> islamabad@deosai.pk</a>
            <a href="planner.html" class="text-success text-decoration-none small mb-0 d-inline-block">Plan Trip &rarr;</a>
          </div>
        </div>
      </div>
    </div>
 </footer>

  <!-- 8. Floating WhatsApp Contact Button -->
  <a href="https://wa.me/923000000000" target="_blank" rel="noopener noreferrer" class="whatsapp-floating-clean" aria-label="Chat on WhatsApp">
    <i class="bi bi-whatsapp"></i>
  </a>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
  <script src="../js/main.js"></script>

  <!-- Page-specific form validation & enquiry summary enhancement (extends main.js without duplicating it) -->
  <script>
    document.addEventListener('DOMContentLoaded', () => {
      const form = document.getElementById('booking-inquiry-form');
      if (!form) return;

      const nameEl = document.getElementById('booking-name');
      const emailEl = document.getElementById('booking-email');
      const phoneEl = document.getElementById('booking-phone');
      const enquiryTypeEl = document.getElementById('booking-subject');
      const subjectEl = document.getElementById('contact-subject');
      const messageEl = document.getElementById('booking-message');
      const errorSummary = document.getElementById('form-error-summary');
      const statusBox = document.getElementById('booking-confirmation');
      const statusWa = document.getElementById('booking-confirm-wa');
      const statusEmail = document.getElementById('booking-confirm-email');

      // Pre-fill Subject if ?tour=... is passed from planner.html or packages/blog pages
      const params = new URLSearchParams(window.location.search);
      const tour = params.get('tour');
      if (tour && subjectEl && !subjectEl.value.trim()) {
        subjectEl.value = `Booking Enquiry: ${tour}`;
      }

      const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
      const phoneRegex = /^[+\d\s()-]{7,20}$/;

      function setFieldState(el, isValid) {
        if (!el) return;
        el.classList.toggle('is-invalid', !isValid);
        el.classList.toggle('is-valid', isValid);
      }
        const emailValid = Boolean(emailEl && emailRegex.test(emailEl.value.trim()));
        const phoneVal = phoneEl ? phoneEl.value.trim() : '';
        const phoneValid = phoneVal === '' || phoneRegex.test(phoneVal);
        const typeValid = Boolean(enquiryTypeEl && enquiryTypeEl.value.trim().length > 0);
        const subjectValid = Boolean(subjectEl && subjectEl.value.trim().length >= 3);
        const messageValid = Boolean(messageEl && messageEl.value.trim().length >= 10);

        setFieldState(nameEl, nameValid);
        setFieldState(emailEl, emailValid);
        if (phoneEl) {
          phoneEl.classList.toggle('is-invalid', !phoneValid);
          phoneEl.classList.toggle('is-valid', phoneValid && phoneVal !== '');
        }
        setFieldState(enquiryTypeEl, typeValid);
        setFieldState(subjectEl, subjectValid);
        setFieldState(messageEl, messageValid);

        const allValid = nameValid && emailValid && phoneValid && typeValid && subjectValid && messageValid;
        if (errorSummary) {
          errorSummary.classList.toggle('d-none', allValid);
        }

        if (!allValid) {
          const firstInvalid = form.querySelector('.is-invalid');
          if (firstInvalid) firstInvalid.focus();
        }

        return allValid;
      }

      // Live feedback clear/update as user edits fields
      [nameEl, emailEl, phoneEl, enquiryTypeEl, subjectEl, messageEl].forEach((field) => {
        if (!field) return;
        const evt = field.tagName === 'SELECT' ? 'change' : 'input';
        field.addEventListener(evt, () => {
          if (field.classList.contains('is-invalid') || field.classList.contains('is-valid')) {
            validateForm();
          }
        });
      });
 // Capture-phase listener runs before main.js's bubble-phase listener so invalid forms do not trigger confirmation
      form.addEventListener('submit', (e) => {
        if (!validateForm()) {
          e.preventDefault();
          e.stopImmediatePropagation();
          if (statusBox) statusBox.classList.add('d-none');
        }
      }, true);

      // Bubble-phase listener runs after main.js to include custom Subject + Enquiry Type and mailto link
      form.addEventListener('submit', () => {
        const name = (nameEl?.value || '').trim();
        const email = (emailEl?.value || '').trim();
        const phone = (phoneEl?.value || '').trim() || 'Not provided';
        const enquiryType = (enquiryTypeEl?.value || '').trim();
        const subject = (subjectEl?.value || '').trim();
        const message = (messageEl?.value || '').trim();

        const summaryBody =
          `Salam DEOSAI Expeditions!\n\n` +
          `• Name: ${name}\n` +
          `• Email: ${email}\n` +
          `• Phone / WhatsApp: ${phone}\n` +
          `• Enquiry Type: ${enquiryType}\n` +
          `• Subject: ${subject}\n` +
          `• Message: ${message}`;

        if (statusWa) {
          statusWa.href = `https://wa.me/923000000000?text=${encodeURIComponent(summaryBody)}`;
        }
        if (statusEmail) {
          statusEmail.href = `mailto:islamabad@deosai.pk?subject=${encodeURIComponent(`[${enquiryType}] ${subject}`)}&body=${encodeURIComponent(summaryBody)}`;
        }
      });
    });
  </script>
</body>
</html>