# FIFA World Cup Dashboard
## Adnan Awad

------

**Link:** https://fifa-world-cup-wins-dashboard.vercel.app/

---

### Description
An interactive dashboard visualizing FIFA World Cup finals history (1930–2022), built with Dash and Plotly. A choropleth map shows total World Cup wins by country, and users can hover any nation to see its exact win count or look up the winner and runner-up for any given tournament year.

2026 World Cup pending. We pray Morocco wins.

Data compiled from Wikipedia's [List of FIFA World Cup finals](https://en.wikipedia.org/wiki/List_of_FIFA_World_Cup_finals).

### Features
- **Choropleth map** of total wins by country, color-scaled so heavier winners stand out at a glance, with exact counts on hover.
- **Winning countries list** — every nation that has ever won the tournament.
- **Yearly finals lookup** — select any World Cup year to see that final's winner and runner-up.

### Design Decisions
- **West Germany / Germany unified:** Pre-1990 West Germany titles are counted under Germany, so the map reflects a single continuous nation rather than splitting historical wins.
- **Hover over color-reading:** Because exact values are hard to read off a color gradient, hovering a country shows its precise win count (`Country (ISO): Wins`) rather than relying on the scale alone.
- **ISO country mapping:** Country names are mapped to ISO-3 codes so Plotly's choropleth can locate them geographically.

### Project Structure
- `app.py` — The Dash application: data setup, choropleth, layout, and interaction callbacks.
- `requirements.txt` — Python dependencies.

### Tech Stack
Python, Dash, Plotly, pandas, Dash Bootstrap Components.

---

## Run Locally

### Prerequisites
Python 3.x installed.

### Setup
1. Navigate to the folder containing `app.py`.
2. Install dependencies:

   `pip install -r requirements.txt`

3. Start the app:

   `python app.py`

4. Open the local address shown in the terminal (usually `http://127.0.0.1:8050/`).