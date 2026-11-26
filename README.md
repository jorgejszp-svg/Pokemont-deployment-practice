# 🔴 Pokémon't · PokéDex OS

**An interactive fan Pokédex with all 1025 Pokémon.** A single-page site built with HTML, Tailwind CSS and vanilla JavaScript. I made it as a class exercise to practise deploying a site: it is served with Nginx next to [PatataRank](https://github.com/jorgejszp-svg/Page-deployment-practice---deployment) on the same port 80, using name-based virtual hosts.

**🔗 Live demo:** https://jorgejszp-svg.github.io/Pokemont-deployment-practice/

## Features

- **Full National Pokédex (1025 Pokémon)** loaded live from [PokeAPI](https://pokeapi.co/), in Spanish, with search, region, type and category filters
- **37 featured entries** with a competitive set, item, nature and tournament notes
- **Detail sheet** with shiny toggle, base stats, abilities, weaknesses and evolution chain
- **Tier list and podium** by total base stats, competitive meta, pseudo-legendaries and starters
- **Versus arena**: hexagon stat radar and an animated turn-based battle at level 50
- **Team builder**: pick 6 Pokémon and get a defensive coverage table, main threats and a team grade
- **Type calculator** for single and dual types
- **"Who's that Pokémon?"** minigame with streak and record
- Captures, team, record, theme and sound are saved in the browser

## Built with

- HTML5
- [Tailwind CSS](https://tailwindcss.com/) via CDN
- Vanilla JavaScript (Web Audio API for the retro sounds)
- [PokeAPI](https://pokeapi.co/) GraphQL endpoint for Pokémon data, cached in `localStorage` for 7 days
- Google Fonts (Fredoka, Nunito and Press Start 2P)

## Run it locally

No build step needed. Clone the repo and open `index.html` in your browser:

```bash
git clone https://github.com/jorgejszp-svg/Pokemont-deployment-practice.git
```

The page needs an internet connection the first time to download the Pokédex. Without it, it falls back to the 37 featured entries.

## Deployment

- **GitHub Pages** from the `main` branch (live demo above).
- **Nginx** on an Ubuntu Server VM from `/srv/pokemont`, as a second virtual host on port 80, published with Cloudflare Tunnel.

## Disclaimer

Non-commercial fan project, not affiliated with Nintendo, Creatures or Game Freak. Pokémon and its characters are trademarks of their respective owners. Data and artwork come from PokeAPI.
