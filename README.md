# Daily Goals

A small daily planner where you add goals, check them off when done and remove them. Each visit shows a random nature photo as background, an inspirational quote and the current weather.

Built with **React 19, TypeScript, Vite, Redux Toolkit and Tailwind CSS 4**.

## Why

Built to practise Redux Toolkit in a realistic setting: one store with several independent slices, each handling its own async data and loading/error state.
- `goalsSlice`: local state (add, toggle, remove goals)
- `backgroundsSlice`: random photos from the Unsplash API, with photographer credit
- `weatherSlice`: current weather from WeatherAPI
- `quotesSlice`: random quote from DummyJSON

All async calls use `createAsyncThunk`.

## Getting started

**Requirements:** Node.js 18+, plus free API keys from [Unsplash](https://unsplash.com/developers) and [WeatherAPI](https://www.weatherapi.com/).

1. Install dependencies:
   ```bash
   npm install
   ```
2. Create a `.env` file in the project root:
   ```env
   VITE_UNSPLASH_ACCESS_KEY=your-unsplash-access-key
   VITE_WEATHER_API_KEY=your-weatherapi-key
   ```
3. Start the dev server:
   ```bash
   npm run dev
   ```
4. Open **http://localhost:5173**.

Other scripts:
```bash
npm run build   # type-check + production build
npm run lint    # ESLint
```

## Tests

No automated tests yet.
