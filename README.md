# Weather in 7 Days

A clean, responsive weather dashboard built with React and TypeScript. Search any city to see current conditions and a 7-day temperature forecast, with light and dark themes.

![React](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-5-646CFF?logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3-06B6D4?logo=tailwindcss&logoColor=white)

## Features

- **Current weather** – temperature, conditions and a matching weather icon for the selected city
- **7-day forecast** – daily temperatures shown on an interactive area chart
- **City search** – look up the weather anywhere in the world
- **Light / dark mode** – switch themes with one click
- **Responsive layout** – works on phones, tablets and large desktop screens

## Tech Stack

| Area        | Tools                                   |
| ----------- | --------------------------------------- |
| Framework   | React 18, TypeScript                    |
| Build tool  | Vite                                    |
| Styling     | Tailwind CSS, shadcn/ui (Radix UI)      |
| Charts      | Recharts                                |
| Icons       | Lucide React                            |
| Data        | [OpenWeatherMap API](https://openweathermap.org/api) |

## Getting Started

### Prerequisites

- Node.js 20 or newer
- A free API key from [OpenWeatherMap](https://home.openweathermap.org/users/sign_up)

### Installation

```bash
# Clone the repository
git clone https://github.com/Ahmad-Nadeem919/My-weather-app.git
cd My-weather-app

# Install dependencies
npm install

# Set up your environment variables
cp .env.example .env
```

Open `.env` and add your OpenWeatherMap key:

```env
VITE_OPENWEATHER_API_KEY=your_api_key_here
```

### Run the app

```bash
npm run dev
```

The app will be available at **http://localhost:8080**.

## Available Scripts

| Command           | Description                             |
| ----------------- | --------------------------------------- |
| `npm run dev`     | Start the development server            |
| `npm run build`   | Type-check and create a production build |
| `npm run preview` | Preview the production build locally    |
| `npm run lint`    | Run ESLint                              |

## Project Structure

```
src/
├── components/
│   ├── WeatherApp.tsx        # Main layout, data fetching, search and theme toggle
│   ├── TemperatureChart.tsx  # 7-day forecast chart
│   ├── WeatherIcon.tsx       # Weather condition icons
│   └── ui/                   # Reusable UI components
├── hooks/                    # Custom React hooks
├── lib/                      # Utility functions
├── pages/
│   ├── Index.tsx
│   └── NotFound.tsx
├── App.tsx
├── main.tsx
└── index.css                 # Theme colors (light / dark)
```

## Deployment

Create a production build with:

```bash
npm run build
```

The output is written to the `dist/` folder and can be deployed to any static host such as Vercel, Netlify or GitHub Pages. Remember to set `VITE_OPENWEATHER_API_KEY` in your hosting provider's environment settings.

## Contributing

Contributions, issues and feature requests are welcome. Feel free to open an issue or submit a pull request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/my-feature`)
3. Commit your changes (`git commit -m "Add my feature"`)
4. Push to the branch (`git push origin feature/my-feature`)
5. Open a pull request

## Author

**Ahmad Nadeem**

- GitHub: [@Ahmad-Nadeem919](https://github.com/Ahmad-Nadeem919)
