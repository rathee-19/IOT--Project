# Hospital Warehouse Management System

This IoT-based web application efficiently manages and tracks the inventory of medical supplies, equipment, and medications in hospital warehouses. It monitors temperature, humidity, and air quality to ensure optimal storage conditions.

## Features

- **Real-Time Monitoring**
  - Displays current temperature, humidity, and air quality status.
  - Alerts for abnormal conditions (e.g., temperature too high/low, air pollution).

- **Inventory Management**
  - Tracks and displays all medicines in the warehouse.
  - Lists expiring medicines.
  - Shows current stock levels.

- **Navigation**
  - Search functionality.
  - Easy access to home, all logs, expiring medicines, and stock indicator pages.

## Setup and Installation

### Prerequisites

- HTML/CSS/JavaScript
- Basic web server (e.g., Apache, Nginx)

### Installation

1. Clone the repository:

    ```sh
    git clone https://github.com/yourusername/hospital-warehouse-management.git
    cd hospital-warehouse-management
    ```

2. Serve the files using your preferred web server or open `index.html` in a browser.

## Project Structure

```
.
├── index.html
├── mainPage.html
├── search.html
├── allLogs.html
├── expiringMedicines.html
├── stockIndicator.html
├── styl.css
├── script.js
└── README.md
```

## Key Components

### `index.html`

- Main entry point, includes links to various sections like home, search, all logs, expiring medicines, and current stock.

### `mainPage.html`

- Displays team name and project overview.

### `search.html`

- Provides search functionality within the warehouse database.

### `allLogs.html`

- Lists all logs of sensor data and inventory changes.

### `expiringMedicines.html`

- Displays medicines that are nearing their expiration date.

### `stockIndicator.html`

- Shows the current stock of all medicines in the warehouse.

### `styl.css`

- Contains the CSS styles for the project.

### `script.js`

- Fetches and displays sensor data from ThingSpeak.
- Manages alerts based on sensor readings.

## Sensors and Data

- **Temperature Sensor**
  - Monitors and displays the current temperature.
- **Humidity Sensor**
  - Monitors and displays the current humidity level.
- **Air Quality Sensor**
  - Monitors and displays the current air quality index.

## Data Fetching

- Uses ThingSpeak API to fetch real-time data from connected IoT sensors.
- Fetch intervals are set to 1 second for temperature, humidity, and RFID data.
- Air quality data is fetched every 10 seconds with alerts for abnormal conditions.

## Contributing

Contributions are welcome! Please create a pull request or open an issue to discuss your ideas.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
