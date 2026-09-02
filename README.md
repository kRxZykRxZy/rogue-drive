# Rogue Drive

A browser-first, fully 3D arcade driving game built with Three.js for CrazyGames.

## Current build
- Full 3D procedural city environment
- Drivable player car with keyboard and mobile touch controls
- Police pursuit AI and heat system
- Health/damage and run-over state
- Cash pickups and score progression
- Persistent garage economy with engine, armour, tyres and nitro upgrades
- Nitro boost
- Responsive HUD and mobile controls
- CrazyGames SDK v3 integration
- CrazyGames gameplay start/stop lifecycle
- CrazyGames midgame ad integration after a run ends

## Run locally
Serve the repository from a local HTTP server because `game.js` uses ES modules:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Controls
- WASD / Arrow keys: drive and steer
- Shift: nitro
- Mobile: on-screen controls

## Production notes
The game currently uses Three.js from jsDelivr to keep the initial repository small. For a final CrazyGames submission, the next pass should add local/bundled Three.js, audio, more vehicle types, missions, better collision physics, more varied city generation, and a rewarded revive/bonus flow. Ads must remain exclusively through the CrazyGames SDK and the game must remain playable when ads are unavailable.
