Meeting Scheduler Bot -- AI Chatbot Instructions Overview The Meeting
Scheduler Bot is designed to engage with users through natural language
to facilitate the scheduling of meetings efficiently. It should interact
with users to understand their commands, extract relevant information,
guide users when data is incomplete, and store all necessary meeting
details in a MySQL database.

Bot Workflow and Functionalities:

Understanding User Input The bot should understand natural language
commands from users, such as:

\"Schedule a meeting with John for tomorrow at 10 AM.\" \"Book a meeting
with the marketing team next Friday.\" It should interpret user input to
extract:

Attendees (names or email addresses) Agenda (purpose of the meeting)
Scheduled time (date and time) Duration (length of the meeting) The bot
should parse these details using natural language processing (NLP) to
understand the user\'s intent.

Collecting Missing Data If any required data is missing, the bot must
prompt the user to provide it. For example:

If the user doesn't provide an agenda: \"What is the agenda for this
meeting?\" If no attendees are mentioned: \"Who will attend the meeting?
Please provide their names or email addresses.\" If no time or date is
specified: \"When would you like to schedule the meeting?\" The bot
should guide the user conversationally, making sure to collect all
necessary details before scheduling.

Handling Ambiguities (Multiple Attendees with the Same Name) When the
bot encounters multiple users with the same name, it should ask for
clarification. For example:

If the user requests, \"Schedule a meeting with John,\" and there are
multiple users named John in the system, the bot should ask: \"There are
multiple contacts with the name John. Could you specify the attendee by
selecting an email: john@example.com or john.smith@example.com?\"
Storing Meeting Information Once all required details are collected, the
bot should store the meeting data in the MySQL database. The information
to be stored includes:

Attendees Agenda Scheduled time Duration The meeting should be
associated with the user who initiated the scheduling. The user ID
should act as a foreign key in the meetings table.

Confirmation Message After the meeting is successfully scheduled, the
bot should confirm with the user by sending a message:

\"Your meeting has been scheduled and updated on your calendar.\" The
confirmation ensures that the user knows their request has been
processed successfully.

Special Scenarios

Missing Data: If the user provides an incomplete request, the bot should
guide them through a series of follow-up questions to collect missing
information. Multiple Users with Same Name: If attendees have the same
name, the bot should ask for clarification, prompting the user to select
the correct individual based on email addresses. Technologies Behind the
Bot:

Django REST API: The backend is powered by Django, where all requests
and responses are processed. MySQL Database: The bot stores user and
meeting data in a MySQL database, ensuring all records are structured.
AI/NLP: The bot uses an open-source AI model to understand and process
user input, extracting relevant data points for scheduling. Bot Behavior
Summary:

Use NLP to understand user commands. Extract key details (attendees,
agenda, time, duration). Prompt the user for missing or unclear
information. Store meeting data in the database. Provide confirmation
once the meeting is successfully scheduled.
