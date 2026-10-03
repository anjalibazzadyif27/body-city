# Body City

Your daily habits, built into a city.

Body City turns your body into a small Indian city. Sleep powers the Control Tower, food keeps the Bazaar open, water fills the River, movement runs the Power Station, mood keeps the Park green, and breaks from sitting keep the Roads moving. A one-minute daily check-in changes the city live.

Built for the Mosaic Wellness x Ashoka University Builder Round.

## Try it

Open `index.html` in any browser, or use the live link. Tap **Explore a demo city** to load three weeks of data for Riya, a final-year student, and see every feature straight away.

## Who it's for

Young Indians, students and early-career professionals, who know they should sleep, eat and move better but give up on number-heavy trackers within a week.

## What it does

- **Daily check-in (about 1 minute):** hours of sleep, glasses of water, katoris of sabzi or fruit, meals with protein, junk items, sweet chais, minutes of movement, mood, stress, and the longest stretch spent sitting. The matching part of the city reacts as you tap.
- **Scored against real guidelines:** every district is scored 0 to 100 against a published guideline, and you can tap any district to see the guideline and its source.
- **Insights:** 7-day averages, days on target, trends, best and worst weekdays, and patterns between your own habits (for example, how sweet chai affects the next night's sleep). Each pattern says how many days it is based on, and that it is a pattern, not proof.
- **7-day repair plan:** one tiny task a day for your weakest district, unlocked daily. Cranes stay over that part of the city until it is rebuilt.
- **Ask the Mayor:** an on-device agent that answers questions like "Why am I tired?" or "What should I fix first?" using your own numbers.
- **Week view and postcard:** seven mini cities, one per day, and a shareable postcard of your city.

## Guidelines used

| District | Habit | Guideline | Source |
|---|---|---|---|
| Control Tower | Sleep | 7 or more hours a night | AASM and Sleep Research Society consensus (2015) |
| Bazaar | Food | About 400 g veg and fruit a day, regular protein foods, limit foods high in fat, sugar and salt; added sugar ideally under about 6 teaspoons | ICMR-NIN Dietary Guidelines for Indians (2024); WHO sugars guideline (2015) |
| River | Water | About 2 L a day for women, 2.5 L for men (total), more in heat | EFSA Dietary Reference Values for water (2010) |
| Power Station | Movement | 150 to 300 minutes of moderate activity a week | WHO Guidelines on Physical Activity and Sedentary Behaviour (2020) |
| Roads | Sitting | Limit long sitting; short walking breaks every 20 to 30 minutes help blood sugar | WHO (2020); Dunstan et al., Diabetes Care (2012) |
| Park | Mood | Self-reported; patterns, not diagnosis. Support: Tele-MANAS 14416 | Ministry of Health and Family Welfare |

## Design decisions

- **Consequences, not numbers.** A dry river or a traffic jam is easier to feel than "4 glasses".
- **Built for India.** Katoris, chai, dal, autos and a banyan tree, not calories and smoothies.
- **On-device Mayor instead of a chatbot.** It needs no login or API, costs nothing, works on any phone, and data never leaves the device. Answers are built from the user's own data and the guidelines above, so it cannot invent unsafe health advice. Mentions of self-harm get the Tele-MANAS helpline and 112; serious symptoms are pointed to a doctor. When the app is opened inside Claude, there is an optional toggle to use Claude for richer answers.
- **Tiny habits.** Repair-plan tasks are small and tied to existing routines, based on BJ Fogg's *Tiny Habits* (2019) and Gollwitzer's work on implementation intentions (1999).

## Tech

A single self-contained HTML file: plain JavaScript, the city drawn in SVG, data stored in the browser's localStorage. No backend, no login, no tracking.

## How AI helped

Built with Claude: brainstorming the idea, designing the city, writing and testing the code, and checking it on desktop and phone screen sizes. I chose the idea, the audience and the features, and pushed for the upgrades from a visual toy to a guideline-based tool with insights, plans and an on-device agent.

*Body City is for awareness, not medical advice.*
