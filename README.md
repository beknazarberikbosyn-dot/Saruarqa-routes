# Saryarqa Routes Prototype

Clickable concept prototype for **Zerttex Hackathon 2026, Stage 1, Case 1: Technology Product**.

Saryarqa Routes is a fictional Astana tour company from the case. The prototype shows how a booking platform with an AI travel assistant would solve the four complaints of foreign guests:

| Guest complaint | Feature in the prototype |
| --- | --- |
| "It is unclear how to book" | 4-step online booking: date, travelers, details, payment |
| "I am not sure the company is trustworthy" | Reviews, guide profiles, licence and refund policy |
| "My foreign card does not work" | Payment options: Visa / Mastercard, Apple Pay, Google Pay, Alipay |
| "I do not know what is included" | "Included / Not included" on every tour page and in the confirmation |

Also included: AI trip planner, AI assistant "Aru the camel" (an animated avatar that opens a chat window when tapped; scripted answers in the demo), language (EN / DE / 中文) and currency (USD / EUR / CNY / KZT) switch.

## 360° route map

- An interactive map (Leaflet + OpenStreetMap) shows all four routes with numbered stops, plus a route map on every tour page.
- Tapping a stop opens a real 360° panorama from Google Street View at that point, with previous / next stop buttons.
- "Open 360° in Google Maps" opens the nearest 360° photo in Google Maps, which helps where Street View has no imagery.
- Stop coordinates are approximate. Edit them in the `POINTS` object in `index.html`.
- The map and panoramas need an internet connection and work on GitHub Pages or any normal web host.

## Getting there

Each tour page lets the traveler pick the arrival city (Almaty or Astana) and how to reach the tour start: plane, train or private car, with approximate time, cost, distance, CO₂ and fuel. Ship is shown as not possible, because no water route reaches these tours. The choice is added to the booking total. Times and prices are approximate estimates for the prototype.

## Food and diet needs

Under "Food on the way and during the trip" the traveler types the group's needs in plain words (English, Chinese or Russian), for example "I'm vegan, my child is allergic to peanuts", or taps tags. The menu follows the chosen travel mode: an airline special-meal code for the plane, dining-car meals for the train, a packed lunch for the car, and guesthouse meals during the tour. Dishes that do not fit are swapped, and the page shows what was replaced and why. Allergies add a warning, because shared kitchens and airlines cannot promise zero traces.

## Documents

When adding travelers, every person uploads a document that confirms name and age: a passport photo page, or a passport or birth certificate for children. A manager checks them within 24 hours, so child and senior prices cannot be misused. In the prototype, files never leave the browser; "Use sample documents (demo)" fills in sample files.

## AI assistant (Aru)

Aru reads the whole question: the tour (also with typos, such as "Charun"), number of days, budget and currency, number of people, transport and food needs. It answers in the language of the question (English, Chinese or Russian), remembers the last tour mentioned, and suggests trips that fit the budget. The answers are still scripted; in the real product the same trip data would go to an AI model.

## Photos

Tour photos are real pictures from Wikimedia Commons, loaded through `Special:FilePath` and credited with links to each file page (author and licence are listed there). If a photo cannot load, the page shows the original illustration instead.

## Important

- This is a demo. Prices, reviews, guides and exchange rates are sample data.
- No real bookings or payments happen. No card details are collected.
- The AI assistant uses scripted answers.
- Exchange rates are fixed: USD from the National Bank rate of 20 October 2026; EUR and CNY are approximate.

## Run

Open `index.html` in a browser, or enable GitHub Pages (Settings → Pages → Deploy from branch → `main` / root).
