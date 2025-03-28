Cold Email Generator
An automated Cold Email Generator designed to help business development executives send personalized cold emails for job applications and client outreach. This tool scrapes job postings, extracts key information, and crafts context-aware cold emails with relevant portfolio links.

Features
Job Posting Scraping: Automatically scrapes job descriptions from provided URLs.
Personalized Email Generation: Crafts cold emails based on extracted job details.
Portfolio Integration: Pulls relevant links from a portfolio stored in a CSV file and includes them in the emails.
Streamlit UI: Provides a simple web interface for input and interaction.
Technologies Used
Python: Main programming language for backend logic.
Streamlit: To create an interactive user interface.
Chroma DB: For storing and querying portfolio data.
Python-dotenv: For secure management of API keys and environment variables.
LangChain: For language model-driven tasks such as extracting job details and writing emails.
How It Works
Input Job URL: The user provides a URL of a job posting.
Job Data Scraping: The app scrapes key details such as job title, required skills, and description from the URL.
Portfolio Query: The portfolio is queried based on the required skills.
Email Generation: The tool generates a cold email using pre-defined templates and includes relevant portfolio links.
Email Display: The generated email is displayed to the user for review.
Installation
Prerequisites:
Python 3.6 or higher
API Key for GROQ (for language model access)
Steps:
Clone the repository:
git clone https://github.com/samarthbillava/cold-email-generator.git

Navigate to the project directory:
cd cold-email-generator
Install the required dependencies:
pip install -r requirements.txt
Create a .env file in the root directory and add your GROQ API Key:
GROQ_API_KEY=your_groq_api_key_here
Usage:
To run the application locally:

Launch the Streamlit app:
streamlit run main.py
Open the URL provided in the terminal to view the app in your browser.
Input:
Enter the URL of a job posting on the Streamlit interface.
Press the Submit button to start the scraping and email generation process.
Output:
The app will display the generated cold email, which can be copied or modified for outreach.
Project Structure
```bash
cold-email-generator/
│
├── main.py               # Main Streamlit app file
├── chain.py              # Contains the logic for extracting job details and generating emails
├── portfolio.py          # Handles portfolio management and querying
├── .env                  # Environment file to store sensitive API keys
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation
```bash
Example
Given a job posting URL like https://jobs.nike.com/job/R-33460, the app scrapes relevant details and generates a personalized email that can be sent as part of your outreach campaign.

Contributing
Fork the repository.
Create a new branch (git checkout -b feature-branch).
Make your changes and commit them (git commit -am 'Add new feature').
Push to the branch (git push origin feature-branch).
Create a pull request.
License
This project is open source and available under the MIT License.

Acknowledgements

GROQ: For providing access to powerful language models.
Streamlit: For making app development easy and interactive.
