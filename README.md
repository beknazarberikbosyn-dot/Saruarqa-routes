# Saryarqa Routes Prototype

Clickable concept prototype for **Zerttex Hackathon 2026, Stage 1, Case 1: Technology Product**.

Saryarqa Routes is a fictional Astana tour company from the case. The prototype shows how a booking platform with an AI travel assistant would solve the four complaints of foreign guests:

| Guest complaint | Feature in the prototype |
| --- | --- |
| "It is unclear how to book" | 4-step online booking: date, travelers, details, payment |
| "I am not sure the company is trustworthy" | Reviews, guide profiles, licence and refund policy |
| "My foreign card does not work" | Payment options: Visa / Mastercard, Apple Pay, Google Pay, Alipay |
| "I do not know what is included" | "Included / Not included" on every tour page and in the confirmation |

Also included: AI trip planner, scripted AI assistant "Aru", language (EN / DE / 中文) and currency (USD / EUR / CNY / KZT) switch.

## 360° route map

- An interactive map (Leaflet + OpenStreetMap) shows all four routes with numbered stops, plus a route map on every tour page.
- Tapping a stop opens a real 360° panorama from Google Street View at that point, with previous / next stop buttons.
- "Open 360° in Google Maps" opens the nearest 360° photo in Google Maps, which helps where Street View has no imagery.
- Stop coordinates are approximate. Edit them in the `POINTS` object in `index.html`.
- The map and panoramas need an internet connection and work on GitHub Pages or any normal web host.

## Photos

Tour photos are real pictures from Wikimedia Commons, loaded through `Special:FilePath` and credited with links to each file page (author and licence are listed there). If a photo cannot load, the page shows the original illustration instead.

## Important

- This is a demo. Prices, reviews, guides and exchange rates are sample data.
- No real bookings or payments happen. No card details are collected.
- The AI assistant uses scripted answers.

## Run

Open `index.html` in a browser, or enable GitHub Pages (Settings → Pages → Deploy from branch → `main` / root).
