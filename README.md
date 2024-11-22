# Football Player Statistics Telegram Bot

A Telegram bot that provides detailed statistics and visualizations for football players using data from fbref.com.

## Contributors
- [ByalykT01](https://github.com/ByalykT01) - Data Visualization & Analysis
- [Exclearf](https://github.com/Exclearf) - Web Scraping & Data Collection

## Features

### Data Collection
- Scrapes player statistics from fbref.com
- Collects basic player info, match statistics, and advanced metrics
- Caches data locally to reduce load on source website
- Handles both field players and goalkeepers

### Visualizations
- Interactive graphs showing player performance over seasons
- Multiple visualization types:
  - Standard statistics (Goals/Assists, Cards)
  - Passing statistics
  - Shooting statistics
  - Goalkeeper-specific statistics (for GKs)
  - Advanced goalkeeper metrics (for GKs)

### Bot Interface
- Search players by name
- View basic player information
- Browse statistics by season
- Navigate through multiple graph types
- Paginated results for better UX

## Technical Details

### Dependencies
- pyTelegramBotAPI
- selenium
- matplotlib
- numpy
- unidecode
- python-dotenv

### Configuration
Configuration options available in `config.ini`:
- Items per page settings
- Browser pool configuration
- Headless mode toggle
- Admin settings

### Setup
1. Install requirements:
```bash
pip install -r reqs.txt
```

2. Configure environment variables:
- Create `.env` file with your Telegram Bot API key
- Adjust `config.ini` as needed

3. Run the bot:
```bash
python src/main.py
```

## Project Structure
- `src/`
  - `data_analyzer/` - Data visualization and analysis
  - `repository/` - Data storage and retrieval
  - `webScraper/` - Web scraping functionality
  - `main.py` - Bot implementation
- `resources/` - Static resources and cached data
- `config.ini` - Configuration file

## License
MIT License
