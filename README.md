# Google Calendar Assistant

Google Calendar Assistant is a streamlined application that leverages LangChain's LangGraph for intelligent scheduling and query management of Google Calendar events. The application interacts with Google Calendar to create, manage, and retrieve events using natural language queries.

## Features
- **Event Creation**: Schedule events based on user instructions.
- **Event Query**: Fetch existing events based on specified dates or times.
- **Free Slot Finder**: Identify available time slots for scheduling new meetings.
- **Natural Language Understanding**: Understand user input and convert it into actionable queries for the calendar.

## Future Enhancements
- Scale to support multiple user calendars.
- Enable user authentication for personalized calendars.
- Integrate with other calendar platforms like Outlook or Apple Calendar.

## Technology Stack
- **Backend**: FastAPI for handling API requests.
- **Frontend**: Streamlit for an interactive user interface.
- **AI Framework**: LangChain's LangGraph for natural language processing.
- **Google Calendar API**: For calendar interactions.

## Deployment
The application is deployed and accessible via:
- **Frontend URL**: [Streamlit app](https://calender-ai-agent-vishnoi-harshi.streamlit.app/)
- **Backend URL**: [FastAPI Backend](https://google-calender-ai-agent.onrender.com)

## Demo Video
Watch the demo video to see the application in action:
[Demo Video](https://www.youtube.com/watch?v=0hvVq1yga_w)

## Prerequisites
- Python 3.8+
- Service Account JSON file for Google Calendar API.
- Environment variables set for API keys.

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
3. Set up `.env` with the following variables:
    ```env
    GOOGLE_API_KEY=your_api_key
    ```
4. Run the backend:
    ```bash
    uvicorn main:app --reload
    ```
5. Launch the frontend:
    ```bash
    streamlit run app.py
    ```

## Usage
- Enter your Google Calendar ID in the Streamlit app.
- Interact with the assistant using natural language queries, such as:
  - "Schedule a meeting tomorrow at 3 PM."
  - "What are my events for today?"
  - "Find free slots for next Monday."

---

## Notes
This application is currently configured to interact with a single Google Calendar (developer-specific). In future iterations, it will scale to support multiple users and calendars dynamically.

