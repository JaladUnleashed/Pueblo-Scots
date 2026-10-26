# Scotland '27 site: gold food + stays update

Deploy: replace `index.html` in the GitHub repo with this one. Netlify republishes in about 30 seconds. The site is one file.

## What changed
- **Gold = food.** Every food panel has a double gold frame, a gold header bar and a crown. Nothing else on the site uses that frame. Pins for food on the maps are gold too.
- **The Gold Eight** (was "The must-try eight") on the front page: numbered, with a legend line ("Gold frame means food"), status chips under each name, a 📞 Book flag, and buttons to each base's Scran tab.
- **Eat here** panel on every base, on the Plan tab and directly under the Map: 👑 Must-eat (bold), 🍽️ Dinner, 🥪 Quick and cheap, 🍺 Pub or pint. Built from the existing food data, so nothing new to maintain.
- **Scran tab** is gold in the sub-nav and its panels use the gold frame.
- **Schedule:** each day gets a gold "Lunch idea / Dinner idea" strip, and 🔑 check-in / 🧳 check-out chips on stay days.
- **Where we sleep:** a front-page card listing all six bases (two booked, four TBC), and a full stay card on the Inverness and Glasgow Plan tabs (photo, dates, cancellation, Take me home button). A compact version sits under each Map.

## Where to edit
- Stay details: the `STAYS` object in `index.html` (search for `const STAYS`). Photos are `STAY_IMG`.
- 📞 Book flags are worked out from the food notes by the `fBook` function. They are a hint, not a booking record.

## Kept off the site on purpose
The site is public, so the Airbnb confirmation code and lockbox/door details are not in the file. They stay in the Airbnb app.

## Open questions
1. Inverness: Airbnb says 4 to 6 Jul, plan says 3 to 5 Jul.
2. Glasgow: dates on the card (11 to 14 Jul) are from the plan, not the booking. Cancellation windows match them, but check.
3. Group size: the crew list has 8 names. Glasgow sleeps up to 7, and Inverness is booked for 7.
