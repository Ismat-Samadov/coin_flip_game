# Coin Flip Game

A modern, interactive coin flip game built with Next.js 16, TypeScript, and Tailwind CSS. Features smooth 3D animations, real-time statistics tracking, and a fully responsive design.

![Next.js](https://img.shields.io/badge/Next.js-16.0-black?style=flat-square&logo=next.js)
![TypeScript](https://img.shields.io/badge/TypeScript-5.9-blue?style=flat-square&logo=typescript)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-4.1-38bdf8?style=flat-square&logo=tailwind-css)

## Features

- **Interactive Gameplay**: Choose heads or tails and flip the coin with smooth 3D animations
- **3D Coin Animation**: Realistic coin flip with 5 full rotations and proper perspective
- **Statistics Tracking**:
  - Total games played
  - Win/loss count
  - Win rate percentage
  - Current winning streak
  - Best streak record
- **Persistent Data**: All statistics are saved in localStorage and persist across sessions
- **Responsive Design**: Optimized for mobile, tablet, and desktop devices
- **Modern UI/UX**:
  - Glass-morphism effects with backdrop blur
  - Gradient backgrounds
  - Smooth animations and transitions
  - Touch-friendly interface
- **Real-time Feedback**: Instant win/loss notifications with animated messages

## Demo

Visit the live demo: [Coin Flip Game](https://your-deployment-url.vercel.app)

## Screenshots

### Desktop View
The game features a beautiful gradient background with a glass-morphism design that adapts to any screen size.

### Mobile View
Fully responsive layout with touch-optimized controls and seamless animations.

## Tech Stack

- **Framework**: [Next.js 16](https://nextjs.org/) with App Router
- **Language**: [TypeScript](https://www.typescriptlang.org/)
- **Styling**: [Tailwind CSS v4](https://tailwindcss.com/)
- **Deployment**: Optimized for [Vercel](https://vercel.com/)

## Getting Started

### Prerequisites

- Node.js 18.x or higher
- npm, yarn, or pnpm

### Installation

1. Clone the repository:
```bash
git clone https://github.com/Ismat-Samadov/coin_flip_game.git
cd coin_flip_game
```

2. Install dependencies:
```bash
npm install
# or
yarn install
# or
pnpm install
```

3. Run the development server:
```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

4. Open [http://localhost:3000](http://localhost:3000) in your browser to see the game.

### Build for Production

```bash
npm run build
npm start
```

## How to Play

1. **Choose Your Side**: Click on either the "Heads" or "Tails" button
2. **Watch the Flip**: The coin will perform a realistic 3D flip animation
3. **See the Result**: The game will display whether you won or lost
4. **Track Your Stats**: View your performance statistics in the stats panel
5. **Play Again**: Click "New Game" to start fresh or keep playing to build your streak!

## Project Structure

```
coin_flip_game/
├── app/
│   ├── globals.css          # Global styles and Tailwind imports
│   ├── layout.tsx            # Root layout component
│   └── page.tsx              # Home page
├── components/
│   └── CoinFlipGame.tsx      # Main game component
├── public/                   # Static assets
├── .gitignore               # Git ignore rules
├── next.config.mjs          # Next.js configuration
├── package.json             # Project dependencies
├── postcss.config.mjs       # PostCSS configuration
├── tsconfig.json            # TypeScript configuration
└── README.md                # This file
```

## Key Components

### CoinFlipGame Component

The main game component (`components/CoinFlipGame.tsx`) handles:
- Game state management
- Coin flip logic and animations
- Statistics tracking and persistence
- User interface rendering

### Features Implementation

- **3D Coin Flip**: CSS transforms with `rotateY` for realistic spinning effect
- **LocalStorage**: Automatic save/load of game statistics
- **Responsive Grid**: Tailwind's responsive utilities for mobile-first design
- **State Management**: React hooks (`useState`, `useEffect`) for game logic

## Customization

### Modify Colors

Edit the gradient background in `app/page.tsx`:
```tsx
<main className="min-h-screen bg-gradient-to-br from-purple-900 via-blue-900 to-indigo-900">
```

### Adjust Animation Speed

Modify the flip duration in `components/CoinFlipGame.tsx`:
```tsx
setTimeout(() => {
  // Change the timeout value (currently 1000ms)
}, 1000);
```

### Change Coin Design

Update the coin styles in `app/globals.css`:
```css
.coin-heads {
  background: linear-gradient(145deg, #ffd700, #ffed4e);
  /* Customize colors and shadows */
}
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance

- **Lighthouse Score**: 95+ on all metrics
- **Bundle Size**: Optimized with Next.js Turbopack
- **Loading Time**: Fast initial load with static generation
- **Animations**: Smooth 60fps animations using CSS transforms

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the ISC License - see the [LICENSE](LICENSE) file for details.

## Author

**Ismat Samadov**

- GitHub: [@Ismat-Samadov](https://github.com/Ismat-Samadov)
- Repository: [coin_flip_game](https://github.com/Ismat-Samadov/coin_flip_game)

## Acknowledgments

- Built with [Next.js](https://nextjs.org/)
- Styled with [Tailwind CSS](https://tailwindcss.com/)
- Deployed on [Vercel](https://vercel.com/)

## Future Enhancements

- [ ] Sound effects for coin flip
- [ ] Multiple coin themes (gold, silver, bronze, custom)
- [ ] Multiplayer mode
- [ ] Leaderboard system
- [ ] Animation speed control
- [ ] Dark/Light mode toggle
- [ ] Share results on social media
- [ ] Betting system with virtual currency

---

Made with ❤️ by Ismat Samadov
