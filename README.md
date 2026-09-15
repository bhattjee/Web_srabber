# Web Scraper

A Flask-based web scraping application that allows users to extract and analyze various elements from websites through a clean, user-friendly interface.

## Features

- **Multi-Element Extraction**: Extract multiple types of data from websites:
  - Images
  - Links (URLs)
  - Favicons
  - Stylesheets (CSS)
  - Scripts (JavaScript)
  - Headings (H1-H6)
  - Meta Tags
  - All data at once

- **Search & Filter**: Filter extracted data using specific search terms (case-insensitive)

- **Modern Web Interface**: Clean, responsive UI with:
  - Intuitive form for URL input
  - Dropdown selection for data types
  - Optional search term input
  - Organized result display with grid layouts

- **Real-time Scraping**: Instant data extraction and display

## Tech Stack

- **Backend**: Flask (Python web framework)
- **HTML Parsing**: BeautifulSoup4
- **HTTP Requests**: Requests library
- **URL Validation**: validators
- **Frontend**: HTML5, CSS3 with responsive design

## Installation

### Prerequisites

- Python 3.7 or higher
- pip (Python package manager)

### Setup

1. Clone the repository:
```bash
git clone <repository-url>
cd Web_Scrabber
```

2. Install required dependencies:
```bash
pip install -r requirements.txt
```

3. Run the application:
```bash
python app.py
```

4. Open your browser and navigate to:
```
http://127.0.0.1:5000
```

## Usage

1. **Enter URL**: Input the website URL you want to scrape (e.g., `https://example.com`)

2. **Select Data Type**: Choose what type of data you want to extract from the dropdown:
   - Images
   - Links
   - Favicons
   - Stylesheets
   - Scripts
   - Headings
   - Meta Tags
   - All Data

3. **Optional Search**: Enter a search term to filter the results (optional)

4. **Click Scrape**: View the extracted data in an organized format

## Project Structure

```
Web_Scrabber/
├── app.py                 # Main Flask application with routes and scraping logic
├── scraper.py             # Additional scraping functions
├── static/
│   └── style.css          # Styling for the web interface
├── templates/
│   ├── index.html         # Homepage with input form
│   └── result.html        # Results display page
├── requirements.txt       # Python dependencies
├── .gitignore            # Git ignore rules
└── README.md             # This file
```

## Dependencies

- Flask
- requests
- beautifulsoup4
- validators

## Security Notes

- This application is intended for educational and legitimate web scraping purposes
- Always respect website `robots.txt` files and terms of service
- Some websites may have anti-scraping measures
- Use responsibly and avoid overwhelming servers with excessive requests

## Limitations

- Dynamic content (JavaScript-rendered) may not be captured
- Some websites may block scraping attempts
- Relative URLs may need additional processing
- Large websites may take longer to scrape

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the MIT License.

## Author

Created as a web scraping tool for data extraction and analysis purposes.

## Disclaimer

This tool should be used responsibly and in compliance with applicable laws and website terms of service. The authors are not responsible for any misuse of this software.
