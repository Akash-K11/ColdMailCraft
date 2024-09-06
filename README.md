# Cold Email Generator

This Streamlit application automates the process of generating personalized cold emails for job opportunities. It uses AI to extract job details from career pages, match them with relevant portfolio items, and create tailored outreach messages.

## Features

- Web scraping of job postings from career pages
- AI-powered job detail extraction
- Portfolio matching based on required skills
- Automated cold email generation
- User-friendly Streamlit interface

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/Akash-K11/ColdMailCraft.git
   cd ColdMailCraft
   ```

2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Set up environment variables:
   Create a `.env` file in the project root and add your Groq API key:
   ```
   GROQ_API_KEY=your_groq_api_key_here
   ```

## Usage

1. Run the Streamlit app:
   ```
   streamlit run main.py
   ```

2. Open your web browser and navigate to the URL provided by Streamlit (usually `http://localhost:8501`).

3. Enter the URL of a job posting in the input field and click "Submit".

4. The app will generate a personalized cold email based on the job details and your portfolio.

## Project Structure

- `main.py`: The main Streamlit application
- `chains.py`: Contains the `Chain` class for AI operations
- `portfolio.py`: Manages the portfolio data and vector store
- `utils.py`: Utility functions for text cleaning
- `app/resource/my_portfolio.csv`: CSV file containing portfolio data

## Dependencies

- Streamlit
- LangChain
- Groq
- ChromaDB
- Pandas
- python-dotenv