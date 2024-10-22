# Meeting Scheduler Project

The **Meeting Scheduler Project** is a chatbot that helps users schedule meetings with ease. It is designed to allow users to schedule meetings through natural language.

The chatbot model should understand user inputs and gather all the necessary information required for scheduling a meeting.

## Necessary Data for Scheduling
The following data is required for scheduling a meeting:

- **Name of the attendees** (or email)
- **Time and date** of the meeting
- **Agenda** (purpose) of the meeting
- **Duration** of the meeting

## Handling Missing Data
If the user input doesn't contain any of the necessary data, the chatbot should prompt the user to provide the missing information:

- If the **attendees** are not mentioned, the model should ask for the name or email of the attendees.
- If the **date and time** of the meeting are not provided, the model should prompt the user for the meeting date and time.
- If the **agenda** of the meeting is missing, the model should request the user to provide the meeting agenda.
- If the **duration** of the meeting is not mentioned, the model should ask for the meeting duration.

## Handling Multiple Attendees with the Same Name
If the user wants to schedule a meeting with an attendee and there are multiple attendees with the same name, the model should ask for the email of the attendee for clarification.
