# ShareVolume

## Project Summary

Your assigned company: Aflac (AFL), CIK 0000004977.

Fetch https://data.sec.gov/api/xbrl/companyconcept/CIK0000004977/dei/EntityCommonStockSharesOutstanding.json (set a descriptive User-Agent per SEC guidance).
Read `.entityName`. Filter `.units.shares[]` for entries whose `fy` > "2020" and
includes a numeric `val`.
Save `data.json` with this structure:
`{"entityName": "Aflac", "max": {"val": ..., "fy": ...}, "min": {"val": ..., "fy": ...}}`
where `max` and `min` refer to the highest and lowest `.val`. Break ties however you like.

Render a visually appealing `index.html` where:
- `<title>` and `<h1>` must include the live `entityName`.
- The max/min figures are clearly marked with these IDs:
  `share-entity-name`,
  `share-max-value`, `share-max-fy`,
  `share-min-value`, `share-min-fy`.

If the page is opened as `index.html?CIK=0001018724` (or any other 10-digit CIK),
`fetch()` from the SEC endpoint for that CIK using any proxy, e.g. AIPipe,
replace every ID listed above and the title and H1 without reloading the page.

Also commit the attachment uid.txt as-is.

**Generated:** 2025-10-22 13:10:59 UTC

## Files

- `LICENSE`
- `index.html`
- `script.js`
- `style.css`
- `uid.txt`

## Setup Instructions

1. Clone this repository:
   ```bash
   git clone <repository-url>
   cd ShareVolume
   ```

2. Open in browser:
   - Simply open `index.html` in your web browser
   - Or use a local server:
     ```bash
     python -m http.server 8000
     # Visit http://localhost:8000
     ```

## Usage

Open the application in a modern web browser. The app will automatically handle the requirements as specified in the project brief.

## Code Explanation

### Main Components

- **index.html**: Main application interface and structure
- **style.css**: Styling and layout (if separate file)
- **script.js**: Application logic and interactivity (if separate file)

The application is built using standard web technologies (HTML5, CSS3, JavaScript) and may include external libraries loaded via CDN for additional functionality.

### Key Features

The application implements all requirements specified in the brief, with proper error handling and user-friendly interface design.

## Technical Details

- Pure client-side application (no backend required)
- External libraries loaded from CDN (no build process needed)
- Responsive design for various screen sizes
- Modern browser required (Chrome, Firefox, Safari, Edge)

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Deployment

This application is deployed on GitHub Pages at the repository's Pages URL.
