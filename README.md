# Anchorage Dog Name Game

A fun web-based game that tests your knowledge of popular dog names in Anchorage, Alaska. Choose between two dog names and guess which one is more commonly registered for dogs in the municipality.

## Features

- **Two difficulty modes**: Easy mode (names with larger popularity differences) and Hard mode (names with very close popularity counts)
- **10-round gameplay** with visual feedback and scoring
- **Dog-themed icons** for each choice using custom Flaticon icons
- **Social sharing** integration for Twitter and Facebook
- **Responsive design** that works on desktop and mobile devices
- **Real data** sourced from Anchorage animal control records

## How to Play

1. Choose between Easy Mode or Hard Mode
2. For each round, select which dog name you think is more popular
3. View the results showing the actual popularity counts
4. Complete 10 rounds to see your final score
5. Share your results on social media or play again

## Local Development

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- No build tools or dependencies required

### Running Locally

1. Clone or download this repository
2. Open `index.html` in your web browser
3. The game will automatically load dog name data and start

The game fetches dog name data from `https://codeforanchorage.org/dog-name-game/dog_names3.json` by default. Local JSON files (`dog_names3.json`, `dogs2.json`) are also available in the repository.

### File Structure

```
├── index.html          # Main HTML file
├── index.js            # Game logic and interactivity
├── styles.css          # Styling and responsive design
├── dogIconClasses.js   # Array of dog icon CSS classes
├── dog_names3.json     # Primary dog name data (name/count pairs)
├── dogs2.json          # Alternative/backup dog name data
├── dog_names_8_10_23.xls # Raw Excel data source
├── resources/
│   └── font/           # Custom Flaticon dog icons
│       ├── Flaticon.eot
│       ├── Flaticon.svg
│       ├── Flaticon.ttf
│       ├── Flaticon.woff
│       ├── _flaticon.scss
│       └── flaticon.html
└── runningDog.gif      # Loading animation
```

## Data Source

The game uses real dog registration data from the Municipality of Anchorage Animal Control. Dog names are converted to lowercase and include registration counts. The data is periodically updated from municipal records.

## Technical Details

- **Frontend**: Vanilla JavaScript, HTML5, CSS3
- **Data Format**: JSON array of objects with `name` and `count` properties
- **Icons**: Custom Flaticon dog icons with CSS classes
- **Analytics**: Google Analytics integration
- **Social Sharing**: Twitter and Facebook sharing with pre-filled messages

## Contributing

This project was created by Code for Anchorage. The game is built with accessibility and simplicity in mind, using semantic HTML and progressive enhancement.

## Links

- [Play Online](https://codeforanchorage.org/dog-name-game/)
- [Code for Anchorage](http://codeforanchorage.org)
- [Adopt a Pet](http://www.muni.org/Departments/health/Admin/animal_control/Pages/AdoptingaPet.aspx)
- [License/Renew Your Dog](http://www.muni.org/Departments/health/Admin/animal_control/Pages/license.aspx)