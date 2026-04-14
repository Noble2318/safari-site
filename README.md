# Safari Site - Tanzania Tours Website

A modern, responsive website for Tanzania safari tours built with React, TypeScript, Vite, and Tailwind CSS.

## Features

- 🏞️ Beautiful safari tour pages (Home, Beach, Safari, Tours, Hotel, Experience, Gallery)
- 📱 Responsive design with Tailwind CSS
- 🎨 Smooth animations with Framer Motion
- 🔄 Code-splitting for optimal performance
- Interactive chatbot component
- 📝 Contact and booking forms

## Tech Stack

- **Frontend**: React 19, TypeScript, Vite
- **Styling**: Tailwind CSS, PostCSS
- **Animations**: Framer Motion
- **Icons**: FontAwesome, Lucide React, React Icons
- **Build Tools**: ESLint, TypeScript

## Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn

### Installation

1. Clone the repository
2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the development server:

   ```bash
   npm run dev
   ```

4. Open [http://localhost:5173](http://localhost:5173) in your browser

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

## Project Structure

```
src/
├── app/
│   ├── ChatBot.tsx
│   └── components/
│       ├── AnimatedText.tsx
│       ├── footer.tsx
│       ├── Logo.tsx
│       └── Navbar.tsx
├── assets/          # Images and static assets
├── page/            # Page components
│   ├── home.tsx
│   ├── beach.tsx
│   ├── safari.tsx
│   ├── tours.tsx
│   ├── hotel.tsx
│   ├── experience.tsx
│   ├── gallery.tsx
│   ├── contact.tsx
│   ├── booking.tsx
│   └── registration.tsx
├── App.css
├── App.tsx
├── index.css
├── layout.tsx
├── main.tsx
└── page.tsx
```

## Performance Optimizations

- Code-splitting with React.lazy and Suspense
- Optimized bundle sizes with Vite
- Lazy loading of page components
- Efficient asset handling

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Run tests and linting
5. Submit a pull request

## License

This project is licensed under the MIT License.
// eslint.config.js
import reactX from "eslint-plugin-react-x";
import reactDom from "eslint-plugin-react-dom";

export default defineConfig([
globalIgnores(["dist"]),
{
files: ["**/*.{ts,tsx}"],
extends: [
// Other configs...
// Enable lint rules for React
reactX.configs["recommended-typescript"],
// Enable lint rules for React DOM
reactDom.configs.recommended,
],
languageOptions: {
parserOptions: {
project: ["./tsconfig.json"],
tsconfigRootDir: import.meta.dirname,
},
// other options...
},
},
]);

```

```
