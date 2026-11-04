<p align="center"><img src="logo.svg" width="72" alt="Boon logo"></p>

# Boon

**Swipe right to pay a real bill for someone, straight to the biller.**

Live demo: https://boonapp.github.io/

Boon is a product prototype. People upload a real bill (electricity, school fees, rent, medical), and patrons swipe through them like a dating app. Swipe right and Face ID pays the biller directly. The person never receives cash, so the money can only go where they said it would.

> Prototype only. No money moves, Face ID is a pretend scan, and identity, bill and screening checks are simulated. Fees and tax rules are simplified summaries as of November 2026, not tax or legal advice.

## What you can try

| Role | What to do |
| --- | --- |
| Patron | Swipe right to grant, left to pass, up to save. Tap a card for the full profile and every charge. Turn on instant grant to skip the review for 30 days. |
| Bill owner | Upload a bill, add an optional profile (what you do now, LinkedIn, GitHub, a website), and send a thank-you note after a grant. |
| Compliance | See bills held by screening or reported by patrons, and release or reject them. |

Keyboard: `←` pass, `→` grant, `↑` save, `I` open the profile.

## What it does

- **Swipe deck with profiles.** Each card shows the bill, the person's city, what they do now, and links patrons can check. Profiles are on by default; any bill owner can switch them off.
- **Every charge upfront.** The card shows the all-in price. The profile sheet breaks it into bill, FX margin, service fee and local tax, plus the exact amount the biller receives and which licensed partner collects and pays out.
- **Verified links.** LinkedIn, GitHub and personal sites are validated (https only, no shorteners, no payment or messaging links) and labelled with how ownership is proven.
- **Fast giving.** Instant grant, saved filters with grant-all, and Gupt Daan (give in secret).
- **Safety built in.** KYC, bill confirmation with the biller, PEP and sanctions screening with fuzzy name matching, sanctioned-region blocks, gift-tax alerts, and a report button.
- **Global.** 67 countries. Detailed tax rules for India, the US, the UK and the eurozone; general guidance and a US$2,000 cap per payment elsewhere.

## Run it

It is one HTML file with no build step.

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000. Data stays in your browser's local storage. "Erase and restore examples" resets it.

## Status

A concept prototype for product review. A real launch needs licensed payment partners in each country, legal sign-off on instant grant and the profile default, real KYC and screening providers, and a trademark search for the name.
