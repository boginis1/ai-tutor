# Scout Simply — Private AI Tutoring

A portable static website for Holly Zoba's private AI tutoring packages.

## Included pages

- `index.html` — Main sales page, prompt comparison, packages, FAQs
- `thank-you-unstuck/index.html` — Unstuck booking page
- `thank-you-ai-tutor/index.html` — AI Tutor first-session booking page
- `thank-you-build-with-me/index.html` — Build-With-Me first-session booking page

## Run locally

No build step, JavaScript framework, database, or API key is needed.

From the repository root:

```sh
python3 -m http.server 8000
```

Open http://localhost:8000 in your browser. Google Fonts loads externally, with system font fallbacks.

## GitHub

Unzip this package and upload its contents to the root of a repository. Include the three page folders. The `.nojekyll` file supports serving this as a plain static site.

Storing the code in GitHub does not move the existing hosted website or automatically synchronize future edits between GitHub and ChatGPT Sites. Deployment and repository visibility are separate choices.

## Hosting elsewhere

Serve the repository root as static files. No build command is required. Navigation on the booking pages uses relative links so the pages also work beneath a repository subpath.

If the website address changes, update the three Stripe Payment Links' after-payment redirects to the corresponding pages at the new address. Leave the existing redirects in place if you are only backing up the code to GitHub.

## Payment and booking links

| Package | Price displayed | Stripe checkout | Calendly |
| --- | --- | --- | --- |
| Unstuck | $195 | https://buy.stripe.com/6oU4gy3aof8Q1c35l3bsc00 | https://calendly.com/holly-41/unstuck-session |
| AI Tutor Pack | $495 | https://buy.stripe.com/28E9ASh1e1i04of4gZbsc01 | https://calendly.com/holly-41/ai-tutor-1st-session |
| Build-With-Me | $2,500 | https://buy.stripe.com/28E6oG26kgcU8Ev4gZbsc02 | https://calendly.com/holly-41/build-with-me-1st-session |

Free fit call: https://calendly.com/holly-41/ai-fit-meeting

The site links to Stripe-hosted checkout and Calendly-hosted scheduling. It does not process card information, verify payments, send welcome emails, or manage session balances. Booking pages are ordinary pages, not payment-gated resources. Stripe settings and Calendly event settings remain in those services and are not exported in this repository.

## Editing

Each HTML file includes its own styling. The main page also contains the JavaScript for the prompt comparison. Update displayed prices and the matching Stripe products together when changing offers.

This export contains the site's files, not its private deployment configuration, credentials, or Git history.
