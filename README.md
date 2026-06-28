# Elves & Orcs

A social deduction game based on the Estonian classic "Kings & Spies".
Figure out who the hidden spies are among your team — before it's too late.

**For**: Friends who enjoy party games, Mafia, Werewolf, or Among Us.

## Play now
[Link to live demo]

## How to play
1. Join a game with friends (3-8 players)
2. Everyone gets a secret role: Elf (good) or Orc (spy)
3. Elves try to identify the spies through discussion and voting
4. Spies try to survive and eliminate the elves
5. The team with the most points at the end wins

## Features
- Digital version of the popular Estonian card game
- No cards needed — everything is in the browser
- Play with friends remotely
- Animated transitions and sound effects
- Dark mode for late-night sessions

## Screenshot
![Gameplay](screenshots/gameplay.png)

## Technical Highlights

- **Stack**: React + TypeScript + Vite + Tailwind CSS
- **State**: Zustand store with devtools and persistence
- **Animations**: Framer Motion for smooth transitions
- **Audio**: Web Audio API for sound effects
- **i18n**: Estonian, English, Russian support
- **Testing**: 58 tests (unit + component)

## Architecture

```
src/
  game/
    logic.ts      # Pure game logic (roles, voting, scoring)
    bot.ts        # AI bot players
    config.ts     # Game configuration (roles, timing)
    sound.ts      # Sound effects and audio management
  store/
    gameStore.ts  # Zustand state store
  i18n/
    index.ts      # Internationalization setup
  App.tsx         # Main app component
```

## License
MIT
