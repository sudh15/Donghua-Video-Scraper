# Donghua Video Extractor V1

Donghua Video Extractor is a Python-based web scraper designed specifically for extracting video details from Donghua streaming sites. It targets sites that host Donghua (Chinese animated series) and extracts essential information such as the post title, Dailymotion video link, and embed code. The results are displayed in a professional grid layout with a simple selection interface.

Note: Only scrap Dailymotion Videos

## Features

- **Targeted Scraping:** Extracts only donghua post links from a given target URL (e.g., `https://animexin.dev/`).
- **Video Details Extraction:** Retrieves the post title, Dailymotion video link, and embed code.
- **Selection Interface:** If multiple posts are found, a selection table titled "Select Link to Scrap" is shown with only the video titles.
- **Copyright Protection:** The code enforces copyright using encrypted values so that the attribution cannot be easily removed.

## Installation

### Requirements
- Python 3.10 or earlier is recommended if using obfuscation tools.
- Flask
- Requests
- BeautifulSoup4

### Setup

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/sudh15/Donghua-Video-Extractor.git
   cd Donghua-Video-Extractor
   ```

2. **Create a Virtual Environment and Install Dependencies:**
   ```bash
   python -m venv venv
   # On Windows:
   venv\Scripts\activate
   # On Unix or MacOS:
   source venv/bin/activate
   pip install -r requirements.txt
   ```
   *Make sure your `requirements.txt` includes:*
   ```
   Flask
   requests
   beautifulsoup4
   ```

3. **Run the Application:**
   ```bash
   python donghua_extractor.py
   ```

4. **Open Your Browser:**
   Navigate to [http://127.0.0.1:5000/](http://127.0.0.1:5000/) to use the extractor.

## Usage

1. **Homepage:**  
   - Enter the target URL (e.g., `https://animexin.dev/`) and click "Scan".
   - Note: This extractor works only on Donghua streaming sites and shows only Dailymotion video sources.

2. **Selection Page:**  
   - If multiple donghua posts are found, a table titled **"Select Link to Scrap"** is displayed with only the video titles and a link labeled "Scrap Details".
   - Click on the desired link to see the full details of that post.

3. **Results Page:**  
   - The results page displays the post’s title, video source, video link, and a copyable embed code (formatted in a professional code box).
   - A back button allows you to return to the selection or index page as appropriate.

4. **Site Information:**  
   - The site info box shows the Target URL, Target Site Name, and Target IP.

## Project Structure

```
Donghua-Video-Extractor/
├── donghua_extractor.py
├── requirements.txt
├── static/
│   └── style.css
└── templates/
    ├── index.html
    ├── select.html
    └── results.html
```

## License

This project is licensed under the MIT License.  
**All copyright notices must remain intact.**

## Disclaimer

Donghua Video Extractor is provided "as-is" without any warranties. Use it at your own risk. The author is not responsible for any misuse or legal issues arising from web scraping.

## Contact

For questions, suggestions, or contributions, please contact me via [email](mailto:sudhanshuthakur15@gmail.com) or visit [Geeta Tech Hub](https://geetatechhub.blogspot.com/).
