# Simple Chatbot - Joey

A rule-based chatbot web application built with Flask for Natural Language Processing coursework.

## Description

This is a simple conversational chatbot named "Joey" that responds to predefined questions and statements using pattern matching. The chatbot provides a web interface where users can have casual conversations on various topics.

## Features

- **Web-based chat interface** with a clean, user-friendly design
- **Rule-based response system** that handles various conversation topics:
  - Personal questions (name, age, personality, hobbies)
  - Greetings and pleasantries
  - Technical questions (programming, chatbots)
  - Casual conversation (weather, music, travel)
  - Humor and witty responses
- **Real-time messaging** with jQuery AJAX
- **Responsive design** with custom CSS styling

## Technologies Used

- **Python 3.x**
- **Flask** - Web framework
- **jQuery** - Frontend interactions
- **SQLite** - Database (db.sqlite3)
- **Gunicorn** - WSGI HTTP Server (for deployment)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/rjmolinag0213r/ChatBoot_Test.git
cd ChatBoot_Test
```

2. Install required dependencies:
```bash
pip install -r requirements.txt
```

## Usage

### Running Locally

Start the Flask development server:

```bash
python app.py
```

The application will be available at `http://127.0.0.1:5000`

### Running with Gunicorn (Production)

```bash
gunicorn app:application
```

## Deployment

This application is configured for deployment on platforms like Heroku using the included `Procfile`.

To deploy on Heroku:

1. Create a new Heroku app
2. Push the code to Heroku:
```bash
git push heroku master
```

## Project Structure

```
simplechatbot/
├── app.py                 # Main Flask application
├── requirements.txt       # Python dependencies
├── Procfile              # Heroku deployment configuration
├── db.sqlite3            # SQLite database
├── static/
│   └── style.css         # Custom CSS styling
└── templates/
    └── index.html        # Chat interface HTML
```

## How It Works

The chatbot uses a simple if-elif-else logic structure to match user input (converted to lowercase) against predefined patterns. When a match is found, it returns a corresponding pre-written response. If no match is found, it returns a default "I do not understand" message.

## Example Conversations

- **User:** "What is your name?"  
  **Joey:** "My name is Joey. Nice to meet you."

- **User:** "How are you?"  
  **Joey:** "I'm fine, thank you for asking. Do you need some help?"

- **User:** "What is your favorite programming language?"  
  **Joey:** "I quite enjoy programming in Python these days."

## Future Enhancements

- Integration with ChatterBot or other NLP libraries for more intelligent responses
- Machine learning-based intent recognition
- Multi-language support
- User authentication and conversation history
- More sophisticated natural language understanding

## Course Information

This project was developed for **CAI3303C Natural Language Processing** at Miami Dade College.

## License

This project is open source and available for educational purposes.

## Author

Ricardo Molina
