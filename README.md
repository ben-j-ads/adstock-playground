# Adstock Playground

An ad keeps working after the week it ran, and the first dollars work harder than the later ones. Slide carryover, saturation and the spend pattern, and watch the effect build up, fade and flatten. A teaching toy for the two ideas behind marketing mix models.

Open `index.html` in any browser. No build step, no dependencies, no network calls.

- **Controls:** spend pattern (one burst, steady, flights), weekly spend, max lift, carryover (geometric adstock), half-saturation and steepness (a Hill curve).
- **Reads out:** the half-life of an ad, total lift over 30 weeks, lift per $1,000 at your spend and at double, and the share of lift that lands after spend stops. The headline is how much more lift doubling the spend buys.
- **Charts:** week-by-week spend, the carryover stock and the resulting lift, plus a diminishing-returns curve for a steady weekly spend with your spend and double marked.
- **Maths:** stock(t) = spend(t) + carryover x stock(t - 1), lift(t) = max x stock^a / (stock^a + half^a), half-life = ln(0.5) / ln(carryover).
- **Share:** a paper-ground PNG card, and the URL hash carries your settings.

This is a toy, not a model. Nothing is estimated from data and the numbers are not benchmarks for any channel. Geometric carryover and a Hill curve are common modelling choices, not facts about your business.

## License

Code is MIT licensed ([LICENSE](LICENSE)). The bundled fonts (Bricolage Grotesque, Archivo) are SIL OFL 1.1, with licenses in `fonts/`. The ben.j.ads wordmark and footnote mark in `logo/` are Ben Johnston's brand assets and are not covered by the MIT license.
