# Travel Tracker

## Overview

Travel Tracker is a web application developed as part of "The Complete Web Development Bootcamp" by Angela Yu. This project leverages Node.js, Express, PostgreSQL, EJS, HTML, CSS, and JavaScript to provide users with an interactive experience where they can input a country name, and that country gets highlighted on a world map displayed on the web page.

## Features

- **Interactive World Map**: Users can input the name of a country, and that country will be colored on the world map.
- **Database Integration**: Uses PostgreSQL to store and retrieve country data.
- **Dynamic User Interface**: Built with EJS for templating and CSS for styling.
- **Responsive Design**: Ensures a smooth user experience across different devices.

## Project Structure

```
TRAVEL TRACKER
│
├── Database
│   ├── countries.csv
│   └── visited_country.csv
│
├── public
│   └── styles
│       └── main.css
│
├── views
│   └── index.ejs
│
├── index.js
└── package.json
```

## Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/MercySpectures/TravelTracker.git
   cd TravelTracker
   ```

2. **Install dependencies**:

   ```bash
   npm install
   ```

3. **Set up PostgreSQL**:
   - Ensure PostgreSQL is installed and running on your machine.
   - Create a database named `LearnPostgreSQL`.
   - Populate the database using the provided `countries.csv` and `visited_country.csv` files.

4. **Configure database connection**:
   Update the database connection details in `index.js`:

   ```javascript
   const db = new pg.Client({
     user: "your-username",
     host: "localhost",
     database: "LearnPostgreSQL",
     password: "your-password",
     port: 5432,
   });
   ```

## Usage

1. **Run the server**:

   ```bash
   npm start
   ```

2. **Open the application**:
   Open your browser and navigate to `http://localhost:3000`.

3. **Track your travels**:
   Enter the name of a country you have visited to see it highlighted on the world map.

## Acknowledgments

- This project was created as part of "The Complete Web Development Bootcamp" by Angela Yu.
- Special thanks to the course instructors and fellow students for their support and guidance.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
