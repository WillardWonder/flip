# Correct Course - GitHub Pages split build

# Structure

- `index.html` - tiny page shell
- `.nojekyll` - keeps GitHub Pages from treating this as a Jekyll site
- `css/game.css` - game styling
- `src/game.js` - main game logic
- `assets/models/meshy-init.js` - global model registry
- `assets/models/*.asset.js` - split Meshy 3D character assets

## Loading behavior

Dean Jason loads immediately because he is always in the game. The selected instructor model loads when that instructor is chosen/played, so the browser does not have to parse every instructor model up front.
