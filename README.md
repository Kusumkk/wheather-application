# Weather Application (Next.js)

React + Next.js version of the weather app. The UI and behavior match the original HTML/CSS/JS app.

## Why Next.js?

- **React** for the UI (search, state, weather display)
- **API route** (`/api/weather`) keeps your OpenWeatherMap key on the server instead of in the browser

## Setup

1. Install dependencies:

   ```bash
   npm install
   ```

2. Add your API key in `.env.local`:

   ```
   OPENWEATHER_API_KEY=your_key_here
   ```

   (A key from the original app is already in `.env.local` for local dev.)

3. Run the dev server:

   ```bash
   npm run dev
   ```

4. Open local host, search for a city, and press Enter.

## Scripts

| Command       | Description              |
|---------------|--------------------------|
| `npm run dev` | Start development server |
| `npm run build` | Production build       |
| `npm start`   | Run production server    |

## Project structure

```
app/
  layout.js          # Root layout + Montserrat font
  page.js            # Weather UI (React client component)
  globals.css        # Styles (from original style.css)
  api/weather/route.js  # Server proxy to OpenWeatherMap
public/
  background.jpg     # Background image
```

## Legacy files

The original `index.html`, `style.css`, and `script.js` are no longer used. You can delete them once you confirm the Next.js app works.
