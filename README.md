# Google Calendar Assistant

Google Calendar Assistant is a streamlined application that leverages LangChain's LangGraph for intelligent scheduling and query management of Google Calendar events. The application interacts with Google Calendar to create, manage, and retrieve events using natural language queries.

## 🚀 Project Overview
A smart AI assistant that helps users schedule meetings through natural language conversations. It interacts via a chat interface, understands time-based requests, checks calendar availability, and confirms bookings.
- **APP LINK**: [link](https://calender-ai-agent-vishnoi-harshi.streamlit.app/)
## 💬 Features
- **Event Creation**: Schedule events based on user instructions.
- **Event Query**: Fetch existing events based on specified dates or times.
- **Free Slot Finder**: Identify available time slots for scheduling new meetings.
- **Natural Language Understanding**: Understand user input and convert it into actionable queries for the calendar.
- **Intent Detection**: Recognizes user intents like scheduling and checking availability.
- **Human-Friendly Parsing**: Parses human-friendly time expressions.
- **Streamlit Chat Interface**: User-friendly chat-based interface.

## 🔧 Technology Stack
- **Frontend**: Streamlit
- **Backend**: Python + FastAPI
- **LLM Used**:Groq:qwen-qwq-32b For fast experience.
- **AI Framework**: LangChain's LangGraph for natural language processing.
- **Calendar Integration**: Google Calendar API
- **Date Parsing**: `dateparser` Python library
- **Secrets Management**: Streamlit Secrets for secure credential storage.
- **Deployment**: Hosted on Streamlit Cloud (frontend) and Render (backend).

## 🔐 Security
- All credentials (API keys, calendar ID, service account) are securely stored using Streamlit’s built-in secrets manager.
- No sensitive files (e.g., `.env` or `.json`) are committed to the repository.

## 📈 Sample Interactions
- “Book a call tomorrow at 3PM.”
- “Do I have any free time this Friday?”
- “Schedule a meeting between 3 and 5 PM next week.”

## 📍 Deployment
The application is deployed and accessible via:
- **Frontend URL**: [Streamlit app](https://calender-ai-agent-vishnoi-harshi.streamlit.app/)
- **Backend URL**: [FastAPI Backend](https://google-calender-ai-agent.onrender.com)

## Demo Video
Watch the demo video to see the application in action:
[Demo Video](https://www.youtube.com/watch?v=0hvVq1yga_w)

## Prerequisites
- Python 3.8+
- Service Account JSON file for Google Calendar API.

## Setup and Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/google-calendar-assistant.git
    cd google-calendar-assistant
    ```
2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Set up Streamlit Secrets:
   - Add your Google Calendar API credentials directly into Streamlit’s built-in Secrets Manager.

4. Run the backend:
    ```bash
    uvicorn main:app --reload
    ```
5. Launch the frontend:
    ```bash
    streamlit run app.py
    ```

## 🧠 Future Improvements
- Add support for cancelling and rescheduling events.
- Implement user authentication (OAuth).
- Enhance memory using LangGraph for multi-turn dialogue.
- Scale to support multiple user calendars.
- Integrate with other calendar platforms like Outlook or Apple Calendar.

## ✅ Outcome
A deployable, secure, and intelligent scheduling agent that demonstrates the power of AI, APIs, and modern cloud tools working together seamlessly.

---

## Notes
This application is currently configured to interact with a single Google Calendar (developer-specific). In future iterations, it will scale to support multiple users and calendars dynamically.
