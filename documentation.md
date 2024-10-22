# Meeting Scheduler Project

The **Meeting Scheduler Project** is a chatbot designed to help users schedule meetings with ease. It allows users to schedule meetings through natural language, and the chatbot's responses should be precise, brief, and on point.

The chatbot model must understand the user's inputs and gather all the necessary information required to schedule a meeting.

## Necessary Data for Scheduling a Meeting:

- **Name of the attendees** (or email)
- **Time and date** of the meeting
- **Agenda** (purpose) of the meeting
- **Duration** of the meeting

### Handling Missing Data

If the user's input does not contain any of the necessary data, the chatbot should prompt the user to provide the missing information. The chatbot should specifically ask for:

- **Attendees**: If the attendees are not mentioned, the model should request the name or email of the attendees.
- **Date and Time**: If the date and time of the meeting are missing, the model should ask for the meeting date and time.
- **Agenda**: If the agenda is not provided, the model should ask for the purpose of the meeting.
- **Duration**: If the user does not mention the duration of the meeting, the model should prompt for a meeting duration.

### Attendee Clarification

If the user wants to schedule a meeting with an attendee and there are multiple attendees with the same name, the model should ask for the attendee's email to clarify the correct participant.
