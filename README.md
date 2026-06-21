# YOUrs Sports & Agency

![Next.js](https://img.shields.io/badge/Next.js-16.1.1-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-19.2.3-149ECA?style=for-the-badge&logo=react&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.4-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![Framer Motion](https://img.shields.io/badge/Framer_Motion-12-0055FF?style=for-the-badge&logo=framer&logoColor=white)

YOUrs Sports & Agency needed a credible digital presence for football player representation across the Italian and Dutch markets.
The result is a bilingual, mobile-first website that presents the agency, its athletes, its services and direct contact paths in a polished Next.js experience.

**Live project:** https://yourssports.com  
**Client / sector:** Sports agency, professional football player representation

## Preview

<p align="center">
  <a href="https://yourssports.com" aria-label="Open the live YOUrs Sports & Agency website">
    <img src="./public/logo.svg" alt="YOUrs Sports & Agency logo" width="220" />
  </a>
</p>

No exported screenshots are committed in this repository. The live deployment is the visual reference for the portfolio review; the most relevant capture points are the localized homepage, the athletes grid and the contact page.

## Tech Stack

| Layer | Tools |
| --- | --- |
| Framework | ![Next.js](https://img.shields.io/badge/Next.js-16.1.1-000000?logo=nextdotjs&logoColor=white) |
| UI | ![React](https://img.shields.io/badge/React-19.2.3-149ECA?logo=react&logoColor=white) ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.4-06B6D4?logo=tailwindcss&logoColor=white) |
| Language | ![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript&logoColor=white) |
| Motion and icons | ![Framer Motion](https://img.shields.io/badge/Framer_Motion-12-0055FF?logo=framer&logoColor=white) ![Lucide](https://img.shields.io/badge/Lucide_React-Icons-F56565?logo=lucide&logoColor=white) |
| Forms | ![React Hook Form](https://img.shields.io/badge/React_Hook_Form-7-EC5990?logo=reacthookform&logoColor=white) ![Zod](https://img.shields.io/badge/Zod-4-3068B7?logo=zod&logoColor=white) |
| Internationalization | `next-intl`, custom `I18nProvider`, localized message catalogs |

## Key Features

- Bilingual routing for Italian and English content, with locale-aware navigation and language switching.
- Athlete portfolio with position filters, profile cards, image assets and Transfermarkt references where available.
- Dedicated agency sections for team, services and mission, structured around player representation, contract support and personal guidance.
- Conversion-focused contact flow with WhatsApp, phone, email and a validated contact form.
- SEO foundation with metadata, localized sitemap entries, robots configuration and `SportsOrganization` JSON-LD.

## Project Structure

The project is built with the Next.js App Router. Locale-specific pages live under `src/app/[locale]`, while the root page redirects to the default Italian locale. `ClientLayout` composes the shared header and footer, and the custom i18n context reads copy from `messages/en.json` and `messages/it.json`.

Reusable UI primitives are kept in `src/components/ui`, layout components in `src/components/layout`, and domain-specific cards in `src/components/players` and `src/components/team`. Athlete, team, contact and site metadata are centralized in `src/lib`, keeping content updates separate from page composition.

## Results and Impact

- Delivered a production-ready website for a real sports agency brand at `yourssports.com`.
- Turned a basic web presence need into a structured portfolio site with clear paths for athletes, clubs and partners.
- Published a searchable catalog of 13 represented athletes with position-based filtering.
- Added bilingual content coverage for the agency's core pages: home, team, players, services and contact.
- Prepared the site for organic discovery through structured metadata, localized routes, sitemap and robots support.

## Local Development

```bash
npm install
npm run dev
```

Open `http://localhost:3000`; the app redirects to `/it` by default.

Useful commands:

| Command | Purpose |
| --- | --- |
| `npm run dev` | Start the local development server |
| `npm run build` | Create a production build |
| `npm run start` | Run the production build locally |
| `npm run lint` | Run ESLint |

## Contact and Portfolio Links

- Live website: https://yourssports.com
- Email: info@yourssport.it
- WhatsApp / phone: +39 3393834099
- Instagram: https://instagram.com/yourssports
- LinkedIn: https://linkedin.com/company/yourssports
- Transfermarkt agency profile: https://www.transfermarkt.nl/yours-sports-amp-agency/beraterfirma/berater/10086
