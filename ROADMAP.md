# CicloMart — Roadmap

Planned work for the CicloMart frontend. Items are grouped by theme; rough effort estimates are in hours.

## Testing & quality
- [ ] Add Vitest + React Testing Library and test the service layer (`src/services/*`) and Redux slices (~8h)
- [ ] Add integration tests for the core flows: registration, login, publish a listing, checkout (~6h)
- [ ] Wire `lint`, `format:check`, `build`, and tests into the GitHub Actions workflow (currently only deploys) (~2h)
- [ ] Add a pre-commit hook (Husky + lint-staged) so formatting/linting run automatically (~1h)

## Type safety
- [ ] Migrate the service layer and Redux slices to TypeScript (~10h)
- [ ] Enable `checkJs` incrementally and replace `prop-types` with TypeScript types (~4h)

## Accessibility & UX
- [ ] Accessibility audit: keyboard navigation, focus states, ARIA labels, and colour contrast across MUI/Tailwind components (~5h)
- [ ] Add a global error boundary and consistent loading/empty/error states (~3h)
- [ ] Improve mobile layouts for the advanced spare-parts filter and product comparison (~4h)

## Internationalisation
- [ ] Finish missing translation keys and add a CI check (extend `check-translations.js`) (~3h)
- [ ] Add a third locale (e.g. Portuguese) (~3h)

## Performance
- [ ] Route-level code splitting with `React.lazy` + `Suspense` (~3h)
- [ ] Replace the large `preview.gif` with a compressed video/screenshot set and lazy-load images (~2h)
- [ ] Audit bundle size and remove unused dependencies (~2h)

## Security & correctness
- [ ] Move Cloudinary uploads to signed uploads (currently unsigned) (~4h)
- [ ] Sanitise user-generated content and validate forms consistently (~3h)
- [ ] Review security headers and the auth/refresh flow for CSRF and token-storage issues (~2h)

## Product features
- [ ] Saved searches and price-drop notifications (~8h)
- [ ] Seller dashboard with sales analytics (~8h)
- [ ] In-app messaging between buyers and sellers (~10h)
