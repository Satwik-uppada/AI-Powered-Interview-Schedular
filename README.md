# AI-Powered Interview Scheduler Bot 🤖

An intelligent interview scheduling system that uses AI to automate the process of finding common available time slots between recruiters and candidates using Google Calendar API.

# Demo

![Image](https://github.com/user-attachments/assets/94a27616-11ed-4c9e-851f-1a2bfad8eed3)

## Features ✨

- **AI-Powered Scheduling**: Automatically finds common free time slots between recruiter and candidate
- **Natural Language Processing**: Understands date and time inputs in natural language
- **Google Calendar Integration**: Seamlessly integrates with Google Calendar for availability checks
- **Interactive UI**: Built with Streamlit for a user-friendly experience
- **Timezone Support**: Handles time slots in IST (Indian Standard Time)
- **Service Account Integration**: Uses Google Cloud service account for secure calendar access

## Prerequisites 📋

Before you begin, ensure you have:

- Python 3.7+
- Google Cloud Platform account
- Google Calendar API enabled
- Service account credentials

## Setup Guide 🛠️

### 1. Google Cloud Platform Setup

1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create a new project or select an existing one
3. Enable the Google Calendar API:
   - Navigate to "APIs & Services" > "Library"
   - Search for "Google Calendar API"
   - Click "Enable"

### 2. Service Account Creation

1. In Google Cloud Console:
   - Go to "APIs & Services" > "Credentials"
   - Click "Create Credentials" > "Service Account"
   - Fill in service account details
   - Click "Create and Continue"
   - Skip role assignment (optional)
   - Click "Done"

2. Generate Service Account Key:
   - Click on the created service account
   - Go to "Keys" tab
   - Click "Add Key" > "Create New Key"
   - Choose JSON format
   - Download the key file

### 3. Project Setup

1. Clone the repository:
```bash
git clone <your-repo-url>
cd ai-powered-scheduling-bot
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Configure credentials:
   - Rename your downloaded service account JSON key to `credentials.json`
   - Place it in the project root directory

### 4. Environment Setup

1. Make sure all required packages are installed:
```bash
pip install streamlit google-api-python-client google-auth-httplib2 google-auth-oauthlib spacy dateparser pandas google-generativeai
```

2. Download spaCy language model:
```bash
python -m spacy download en_core_web_sm
```

## Running the Application 🚀

1. Start the Streamlit app:
```bash
streamlit run app.py
```

2. Access the application at `http://localhost:8501`

## Project Structure 📁

```
├── Bot.py               # Bot logic and Implementation
├── requirements.txt     # Project dependencies
└── credentials.json     # Google Cloud service account credentials
```

## Technical Details 🔧

- **Framework**: Streamlit for web interface
- **APIs**: Google Calendar API for scheduling
- **Authentication**: Service Account for secure access
- **NLP**: spaCy for natural language processing
- **AI Model**: Google's Gemini API for intelligent interactions
- **Date & Time Management**: dateparser for natural date parsing

## Security Considerations 🔒

- Service account credentials are required for calendar access
- OAuth 2.0 authentication flow for secure API access
- Separate configurations for development and production
- Secure handling of sensitive credentials

## Contributing 🤝

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License 📄

This project is licensed under the MIT License - see the LICENSE file for details.

## Support 💁

For support and queries, please open an issue in the repository.
