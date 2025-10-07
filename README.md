<p align="center">
    <h1 align="center">HAYYat_DSU Sentiment Analysis Engine</h1>
</p>
<p align="center">
    <em>A Flask web application that scrapes online sources (News, Twitter, YouTube) for multi-source sentiment analysis on user-defined topics.</em>
</p>
<p align="center">
	<img src="https://img.shields.io/github/license/althaf803/HAYYat_DSU?style=flat&logo=opensourceinitiative&logoColor=white&color=0080ff" alt="license">
	<img src="https://img.shields.io/github/last-commit/althaf803/HAYYat_DSU?style=flat&logo=git&logoColor=white&color=0080ff" alt="last-commit">
	<img src="https://img.shields.io/github/languages/top/althaf803/HAYYat_DSU?style=flat&color=0080ff" alt="repo-top-language">
	<img src="https://img.shields.io/github/languages/count/althaf803/HAYYat_DSU?style=flat&color=0080ff" alt="repo-language-count">
</p>

---

## ▶️ Overview

HAYYat_DSU is a comprehensive sentiment analysis tool built with Python and Flask. It allows users to input search queries to scrape real-time data from news articles, Twitter (X), and YouTube comments. The collected data is then processed through a sophisticated sentiment analysis pipeline using models from Hugging Face Transformers and other NLP libraries. The final results, including sentiment scores and source links, are displayed on a clean and interactive web interface.

This project demonstrates a full-stack approach, combining backend data processing with a dynamic frontend to deliver insights on public opinion.

---

## ✨ Features

-   **Multi-Source Scraping**: Gathers data from Google News, Twitter (via search and user profiles), and YouTube comments.
-   **Advanced Sentiment Analysis**: Utilizes a powerful pipeline including `transformers`, `spaCy`, and `NLTK` for accurate sentiment scoring.
-   **Web-Based Interface**: A simple and intuitive UI built with Flask, HTML, and CSS for easy interaction.
-   **Modular Architecture**: The project is broken down into distinct modules for data collection, sentiment analysis, and web presentation, making it easy to maintain and extend.
-   **Dynamic Results Display**: Presents the analyzed data in a clear card-based layout on the results page.

---

## 🛠️ Built With

The project is built with the following major frameworks, libraries, and tools:

<p align="left">
	<img src="https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=Python&logoColor=white" alt="Python">
	<img src="https://img.shields.io/badge/Flask-000000.svg?style=flat&logo=Flask&logoColor=white" alt="Flask">
	<img src="https://img.shields.io/badge/Selenium-43B02A.svg?style=flat&logo=Selenium&logoColor=white" alt="Selenium">
	<img src="https://img.shields.io/badge/Beautiful%20Soup-A06544.svg?style=flat&logo=Beautiful-Soup&logoColor=white" alt="Beautiful Soup">
	<img src="https://img.shields.io/badge/pandas-150458.svg?style=flat&logo=pandas&logoColor=white" alt="pandas">
	<img src="https://img.shields.io/badge/Hugging%20Face-FFD21E.svg?style=flat&logo=Hugging-Face&logoColor=black" alt="Hugging Face">
	<img src="https://img.shields.io/badge/spaCy-09A3D5.svg?style=flat&logo=spaCy&logoColor=white" alt="spaCy">
	<img src="https://img.shields.io/badge/NLTK-3776AB.svg?style=flat&logo=NLTK&logoColor=white" alt="NLTK">
	<img src="https://img.shields.io/badge/Jupyter-F37626.svg?style=flat&logo=Jupyter&logoColor=white" alt="Jupyter">
	<img src="https://img.shields.io/badge/HTML5-E34F26.svg?style=flat&logo=HTML5&logoColor=white" alt="HTML5">
	<img src="https://img.shields.io/badge/JavaScript-F7DF1E.svg?style=flat&logo=JavaScript&logoColor=black" alt="JavaScript">
</p>

---

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.

### Prerequisites

-   **Python**: Version `3.8` or newer.
-   **Google Chrome**: The project uses Selenium to automate Chrome, so it must be installed.
-   **Git**: Required for cloning the repository.

### Installation

1.  **Clone the Repository**
    ```sh
    git clone [https://github.com/althaf803/HAYYat_DSU.git](https://github.com/althaf803/HAYYat_DSU.git)
    cd HAYYat_DSU
    ```

2.  **Create and Activate a Virtual Environment**
    ```sh
    # Create the environment
    python -m venv venv

    # Activate on Windows
    .\venv\Scripts\activate
    ```

3.  **Install Required Dependencies**
    Install all necessary libraries using the `requirements.txt` file.
    ```sh
    python -m pip install -r requirements.txt
    ```

4.  **Download NLP Models**
    The project requires data models for `spaCy` and `NLTK`.
    ```sh
    python -m spacy download en_core_web_sm
    python -c "import nltk; nltk.download('stopwords')"
    ```
5.  **Configuration (Crucial Steps)**
    * **Twitter Credentials**: Add your Twitter (X) username and password in `src/data_collection/twitter_news/twitter_details.py`.
    * **YouTube API Key**: Generate your own YouTube Data API v3 key from the Google Cloud Console and add it to `src/data_collection/scrape_yt_comments/get_yt_comments.py`.
    * **WebDriver**: Download the `chromedriver.exe` that matches your version of Google Chrome and place it in the correct directory as specified in the scraper scripts (e.g., `src/data_collection/`).

### Usage

To run the Flask application:

1.  Navigate to the `src` folder from the project's root directory:
    ```sh
    cd src
    ```

2.  Run the Flask application:
    ```sh
    python app.py
    ```

3.  Open your web browser and go to `http://127.0.0.1:5000`.

---

## 🗺️ Project Roadmap

-   [X] <strike>Core scraping and analysis engine for News, Twitter, and YouTube.</strike>
-   [X] <strike>Flask web interface for user input and results display.</strike>
-   [ ] Improve scraper resilience to handle website blocks and CAPTCHAs.
-   [ ] Implement a database (e.g., SQLite, PostgreSQL) to store historical search results.
-   [ ] Enhance frontend with better data visualizations (e.g., charts, graphs).
-   [ ] Refactor code to use a centralized configuration for API keys and paths.

---

## 🤝 Contributing

Contributions are welcome! Here are several ways you can contribute:

-   **[Report Issues](https://github.com/althaf803/HAYYat_DSU/issues)**: Submit bugs found or log feature requests.
-   **[Submit Pull Requests](https://github.com/althaf803/HAYYat_DSU/pulls)**: Review open PRs, and submit your own.
-   **[Join the Discussions](https://github.com/althaf803/HAYYat_DSU/discussions)**: Share your insights, provide feedback, or ask questions.

---

## 📜 License

This project is licensed under the **MIT License**. You can create a `LICENSE` file in your repository and add the MIT License text to it.

---

## 🙏 Acknowledgments

-   Acknowledge any resources, inspirations, or contributors here.