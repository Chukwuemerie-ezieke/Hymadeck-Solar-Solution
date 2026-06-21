# AGENTS.md

## Project purpose
This repository contains the website for Hymadeck Solar Solution. The site should present the company as a premium, trustworthy, business-grade solar solutions provider and should be improved over time into a full ecommerce-enabled website.

Hymadeck Solar Solution provides:
- Solar procurement
- Solar installation
- Solar maintenance
- Renewable energy solutions for residential, commercial, and industrial clients

The immediate goal is to upgrade the website so it looks more advanced, more professional, and more credible for real business use. The medium-term goal is to make it ecommerce-ready and then fully ecommerce-capable.

## Business goals
The website should help the business:
- Look credible to serious clients
- Generate enquiries and quote requests
- Support WhatsApp, phone, email, and contact form conversion
- Present products and services clearly
- Showcase projects and trust signals
- Support future online sales of products and service packages

## Current context
- The existing website may be a plain static HTML/CSS site.
- Some parts of the current content may be placeholders.
- Do not assume missing business details.
- Where real information is missing, use clearly marked placeholders.
- Do not invent certifications, testimonials, office addresses, customer counts, years of experience, or project statistics.

## Required tone and writing style
Use plain professional language.

Rules:
- Avoid AI buzzwords
- Avoid marketing fluff
- Avoid technical jargon where simpler wording works
- Avoid em dashes
- Avoid exaggerated claims
- Avoid generic hero text like "empowering your future" or "unlocking innovation"
- Be specific, practical, and businesslike

Good examples:
- "Solar systems designed for homes, businesses, and industrial facilities"
- "Request a consultation"
- "Procurement, installation, and maintenance in one delivery model"

Bad examples:
- "Revolutionizing the future of clean energy"
- "Cutting-edge innovative solutions for tomorrow"
- "World-class best-in-class platform"

## Design direction
The site should feel:
- Premium
- Clean
- Modern
- Reliable
- Business-grade
- Calm and confident

Avoid:
- Cheap template feel
- Cluttered layouts
- Overuse of gradients
- Too many accent colors
- Cartoonish icons
- Generic AI-looking sections
- Weak visual hierarchy

Preferred design qualities:
- Strong spacing and alignment
- Clear typography hierarchy
- Professional hero sections
- Clean cards and content blocks
- Strong trust and conversion sections
- Consistent header and footer
- Mobile-first responsiveness

## Functional direction
The site should evolve in phases.

### Phase 1
Premium business website with:
- Home
- About
- Services
- Projects or Case Studies
- Contact
- FAQ
- Testimonials or trust section
- Quote request flow
- WhatsApp call to action

### Phase 2
Ecommerce-ready structure with:
- Shop page
- Product category views
- Product detail pages
- Cart page
- Checkout page UI
- Product cards
- Service package purchase or enquiry flow
- Search and filtering if practical

### Phase 3
Full ecommerce enablement with:
- Payment integration
- Order handling
- Inventory logic
- Admin/product management
- CRM or lead workflow integrations

## Engineering rules
Before changing code:
1. Inspect the current repository structure.
2. Identify reusable parts.
3. Create a plan.
4. Keep changes organized and maintainable.
5. Prefer practical improvements over large unnecessary rewrites.

General coding rules:
- Keep code readable and modular.
- Reuse shared components where practical.
- Do not break existing navigation unless replacing it cleanly.
- Preserve deployability at all times.
- Keep filenames clear and descriptive.
- Keep HTML semantic.
- Keep CSS organized and consistent.
- Keep JavaScript focused and minimal where possible.
- Avoid unnecessary dependencies.

If recommending a framework migration:
- Explain why
- Explain the tradeoffs
- Explain the migration path
- Do not migrate blindly

## Content rules
When writing or rewriting content:
- Keep the company positioning grounded and credible
- Focus on customer value, trust, and clarity
- Do not fabricate client names or reviews
- Do not fabricate case studies
- Do not fabricate product brands unless explicitly provided
- Mark placeholders clearly where real content is needed

If placeholder content is necessary, label it clearly, for example:
- [Placeholder phone number]
- [Placeholder business address]
- [Add real testimonial here]
- [Add actual project images here]

## SEO and performance rules
Every meaningful update should consider:
- Clear page titles
- Useful meta descriptions
- Semantic heading structure
- Good mobile responsiveness
- Reasonable page speed
- Optimized images where practical
- Clean internal linking
- Accessible forms and buttons

## Ecommerce rules
If ecommerce is added:
- Keep the user journey clear
- Support both product sales and service enquiries where appropriate
- Make pricing and calls to action easy to understand
- Keep cart and checkout layouts professional and simple
- Do not fake payment success flows as if they are live when they are only UI prototypes
- Clearly separate frontend prototype behavior from real backend functionality

## Deployment assumptions
Unless told otherwise:
- Keep the project deployable as a static site if possible
- Do not require a backend for basic presentation improvements
- If advanced ecommerce needs a backend or SaaS integration, document that clearly
- Keep deployment notes updated when major structural changes are made

## Expected outputs from coding agents
For substantial tasks, provide:
1. Short assessment of current state
2. Implementation plan
3. Files to be changed or added
4. Code changes
5. Summary of what was completed
6. List of placeholders still needing client input
7. List of next steps for full production readiness

## Priority order
When making decisions, prioritize in this order:
1. Business credibility
2. Clear conversion paths
3. Clean user experience
4. Maintainable code
5. Performance and SEO
6. Ecommerce readiness
7. Nice-to-have animation or visual polish

## Non-negotiables
- Do not invent facts
- Do not use hype-filled copy
- Do not add bloat for its own sake
- Do not break the existing site without replacing it cleanly
- Do not ship confusing placeholder logic as if it is live production functionality
- Do not remove working content unless there is a clearly better replacement

## Default task behavior
When given a task, the coding agent should:
- Review the repository first
- State understanding of the business goal
- Propose a concise plan
- Then implement carefully
- Leave a clear summary of changes and unresolved items
