# 💼 Dice.com Job Scraper

A powerful and user-friendly Streamlit web application that scrapes job listings from Dice.com with advanced filtering options and data export capabilities.

## 🌟 Features

- **🔍 Smart Job Search**: Search for jobs by title with intelligent query processing
- **🎯 Easy Apply Filter**: Toggle between Easy Apply jobs only or all available positions
- **📊 Interactive Results Table**: View job listings in a clean, sortable table format
- **📥 Excel Export**: Download your search results as a professionally formatted Excel file
- **⚡ Real-time Progress**: Live progress tracking during the scraping process
- **📈 Summary Statistics**: Get insights on total jobs, companies, remote positions, and Easy Apply jobs
- **🔗 Clickable Links**: Direct links to job postings for easy application
- **📱 Responsive Design**: Works seamlessly on desktop and mobile devices

## 🚀 Live Demo

[🌐 Try the App Live](https://dicejobsearch.streamlit.app/)

## 📸 Screenshots

### Main Interface
![Main Interface](https://github.com/No0Bitah/dice_job_search/blob/main/screenshots/main_interface.png)

### Results Table
![Results Table](https://github.com/No0Bitah/dice_job_search/blob/main/screenshots/result.png)

## 🛠️ Installation & Setup

### Prerequisites
- Python 3.7 or higher
- pip package manager

### Local Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/No0Bitah/dice_job_search.git
   cd dice_job_search
   ```

2. **Create a virtual environment** (recommended)
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the application**
   ```bash
   streamlit run app.py
   ```

5. **Open your browser** and go to `http://localhost:8501`

## 📦 Dependencies

- **streamlit** >= 1.28.0 - Web framework for the user interface
- **pandas** >= 1.5.0 - Data manipulation and analysis
- **requests** >= 2.28.0 - HTTP library for web scraping
- **beautifulsoup4** >= 4.11.0 - HTML parsing and web scraping
- **python-dateutil** >= 2.8.0 - Date parsing utilities
- **openpyxl** >= 3.0.0 - Excel file creation and manipulation
- **lxml** >= 4.9.0 - XML and HTML processing

## 🎯 How to Use

1. **Enter Job Title**: Type the position you're looking for (e.g., "Python Developer", "Data Scientist", "Software Engineer")

2. **Set Number of Jobs**: Choose how many job listings you want to scrape (1-100)

3. **Toggle Easy Apply Filter**: 
   - **ON** (default): Only shows jobs with Easy Apply feature
   - **OFF**: Shows all available jobs from Dice.com

4. **Click Search**: The app will start scraping jobs with real-time progress updates

5. **View Results**: Browse jobs in an interactive table with sorting and filtering capabilities

6. **Download Excel**: Click the download button to save results as an Excel file

## 📊 Data Fields

Each job listing includes the following information:

| Field | Description |
|-------|-------------|
| **Job Title** | The position title |
| **Company** | Hiring company name |
| **Location** | Job location (including remote options) |
| **Position Type** | Full-time, Contract, Part-time, etc. |
| **Compensation** | Salary range or hourly rate (when available) |
| **Date Posted** | When the job was originally posted |
| **Application** | "Easy Apply" or "External Apply" |
| **Job Link** | Direct link to the job posting |
| **Job Description** | Full job description and requirements |

## ⚙️ Technical Details

### Architecture
- **Frontend**: Streamlit for the user interface
- **Backend**: Custom web scraping engine with concurrent processing
- **Data Processing**: Pandas for data manipulation and Excel export
- **Web Scraping**: BeautifulSoup4 + Requests with user agent rotation

### Performance Features
- **Parallel Processing**: Concurrent job detail fetching for faster results
- **Caching**: LRU cache for repeated URL requests
- **Rate Limiting**: Built-in delays to respect Dice.com's servers
- **Error Handling**: Robust error handling with user-friendly messages

### Ethical Scraping
- Randomized user agents to distribute requests
- Built-in delays between requests
- Respects robots.txt guidelines
- No excessive server load

## 🚀 Deployment

### Streamlit Community Cloud (Free)

1. **Fork/Clone** this repository to your GitHub account

2. **Visit** [share.streamlit.io](https://share.streamlit.io)

3. **Connect** your GitHub account

4. **Select** your repository and set:
   - **Main file path**: `app.py`
   - **Python version**: 3.9+ (recommended)

5. **Deploy** and get your public URL!

### Other Deployment Options
- **Heroku**: Platform-as-a-Service deployment
- **Railway**: Modern deployment platform
- **Render**: Easy web service deployment
- **Docker**: Containerized deployment option

## 🛡️ Limitations & Considerations

- **Rate Limiting**: The app includes built-in delays to avoid overwhelming Dice.com's servers
- **Dynamic Content**: Some job details may not be captured if they're loaded dynamically
- **Site Changes**: Dice.com may update their structure, which could affect scraping
- **Legal Compliance**: Always ensure your usage complies with Dice.com's Terms of Service

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### Areas for Improvement
- Add more job boards (Indeed, LinkedIn, etc.)
- Implement job alerts and notifications
- Add advanced filtering options
- Create data visualization dashboards
- Improve mobile responsiveness

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⚠️ Disclaimer

This tool is for educational and personal use only. Users are responsible for ensuring their usage complies with Dice.com's Terms of Service and applicable laws. The developers are not responsible for any misuse of this application.

## 📞 Support

- **Issues**: [GitHub Issues](https://github.com/No0Bitah/dice_job_search/issues)
- **Discussions**: [GitHub Discussions](https://github.com/No0Bitah/dice_job_search/discussions)
- **Email**: jomari.daison@gmail.com

## 🙏 Acknowledgments

- **Streamlit Team** for the amazing framework
- **Dice.com** for providing job listings data
- **Open Source Community** for the excellent libraries used in this project

## 📈 Roadmap

- [ ] Add support for more job boards
- [ ] Implement job matching algorithms
- [ ] Create mobile app version
- [ ] Add data visualization features
- [ ] Implement user accounts and job tracking
- [ ] Add API endpoints for integration

---

**Made with ❤️ by [No0Bitah](https://github.com/No0Bitah)**

*If you find this project helpful, please give it a ⭐ on GitHub!*
