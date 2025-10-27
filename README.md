# San Francisco Film Locations - Interactive Map

An interactive visualization of film locations in San Francisco using dynamic queries and D3.js.

## How to Use

### Running Locally

1. Make sure you have all files in the same directory:

   - `index.html`
   - `sf_map.png`
   - `SF_Film_Locations_Filtered.csv`

2. Start a local web server:

```bash
python -m http.server 8000
```

3. Open your browser and navigate to:

```
http://localhost:8000
```

### Using GitHub Pages

1. Push this repository to GitHub
2. Enable GitHub Pages in repository settings
3. Your site will be live at: `https://yourusername.github.io/repository-name/`

## Features

### 🎯 Dynamic Query Circles

- **Circle A (Blue)** and **Circle B (Orange)**: Drag the circles to move them around the map
- Adjust the radius using the sliders - locations within both circles are highlighted
- Locations outside the intersection are grayed out

### 📅 Year Range Filter

- Use the min/max year sliders to filter films by release year

### 🎬 Director Filter

- Multi-select dropdown to filter by director
- Hold Ctrl (Cmd on Mac) to select multiple directors
- Leave empty to show all directors

### 🖱️ Interactive Tooltips

- Hover over any film location to see:
  - Film title
  - Release year
  - Location address
  - Actors (Actor 1, 2, 3)
  - Director and writer
  - Production company and distributor
  - Fun facts (when available)

## Technical Details

- **D3.js v7** for visualization and interactions
- **Mercator projection** fitted to San Francisco map bounds
- **Haversine formula** for accurate distance calculations
- Updates at interactive rates (< 0.1s) even with ~2000 data points
- Responsive SVG map with custom styling

## Files

- `index.html` - Main application file
- `sf_map.png` - San Francisco base map image
- `SF_Film_Locations_Filtered.csv` - Dataset with film locations
- `README.md` - This file
# a3
