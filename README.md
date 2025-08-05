# Weather App

This is a front-end-only React weather app built as a homework assignment for OneLegal. It fetches weather data from the National Weather Service API based on user-inputted city/state info.

**Live Demo:** [http://bensmash.net/oneLegal/](http://bensmash.net/oneLegal/)

---

## How to Run

No installation required — it's live and ready to go. Just visit the link above.

---

## Overview

About two weeks ago, I hadn't touched React. One week ago, I finished a couple of React courses on LinkedIn. This past weekend, I started building this project — my very first React app.

I began by asking ChatGPT for a basic React implementation that would pull the current temperature from the National Weather Service API. That initial scaffold helped me understand how to structure API calls in React. From there, I built out:

- An input field to get user location
- API data handling for temperature, wind speed/direction, forecast, etc.
- A visual layout that includes a map and a star chart for the provided location
- Clean UI/UX using Bootstrap for responsiveness

---

## Design Decisions & Assumptions

- **Dark theme & color palette:** Chose purple/pink tones for contrast and readability
- **Data hierarchy:** Prioritized current conditions over forecast data
- **Wind direction icon:** Built a custom SVG that rotates based on compass direction
- **Forecast grouping:** Collapsed 14 time periods (7 days × day/night) into 7 daily summaries
- **Layout compromise:** Used Bootstrap’s 12-column grid, even though it doesn’t divide cleanly into 7 — hence, one “straggler” day drops to a second row
- **Temperature chart:** Used Recharts (with help from ClaudeAI) for a responsive line graph
- **Location prettifying:** Added logic to reformat input like “tempe, az” into “Tempe, AZ”

---

## Features

- Live temperature, wind, forecast, and weather icon
- Map centered on user-inputted location
- Star chart of the current night sky for that location
- 7-day forecast (grouped by day)
- Responsive UI
- Animated wind direction icon

---

## Future Improvements

With more time, I'd love to:

- Let users **save favorite locations**
- Clean up the **7-day layout** (especially on small screens)
- Swap the static map for a **live radar map** with weather overlays
- **Color-code wind icon** based on wind speed (green/yellow/red)
- Add **weather alerts** for conditions like tsunamis, tornadoes, etc.
