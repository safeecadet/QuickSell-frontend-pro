This project is an interactive Kanban board built with React JS, designed to work with the provided API to display and manage tickets. It allows users to dynamically group and sort tickets, with a responsive design that ensures a seamless experience across devices. The application also saves the user's view settings, such as grouping and sorting preferences, so they remain intact after a page reload.

Overview
The Kanban board connects to the API at https://api.quicksell.co/v1/internal/frontend-assignment to retrieve ticket data. Users can organize tickets by grouping them based on status, user, or priority, and sort them by either priority or title. The design is fully responsive, and the user's settings (grouping and sorting preferences) are stored locally, ensuring they persist even after refreshing the page.

Features
Grouping:

Group tickets by Status, User, or Priority.
Sorting:

Sort tickets by Priority (highest to lowest) or by Title (alphabetically).
Responsive Design:

Optimized for different devices, providing a smooth experience whether on desktop or mobile.
Persistent View State:

Saves the user’s grouping and sorting preferences so that the same view is restored after reloading the page.
API
The board communicates with the following API:

Endpoint: https://api.quicksell.co/v1/internal/frontend-assignment

The API provides ticket information with various properties, including:

Status: Current status of the ticket (e.g., Todo, In Progress, Done).
User: The assigned user for the ticket.
Priority: The ticket’s priority level, ranging from 0 to 4.
Priority Levels:

0: No Priority
1: Low
2: Medium
3: High
4: Urgent
Usage
Displaying Tickets: On application load, users can click the "Display" button to fetch and show tickets from the API.
Grouping: Users can select a grouping option (Status, User, or Priority) from a dropdown to organize the tickets.
Sorting: After grouping, users can choose to sort tickets by either Priority (descending) or Title (ascending).
View Persistence: The application retains the selected grouping and sorting settings even after the page is refreshed.
Example UI Flow
Select Grouping: After clicking "Display," the user can group tickets by Status, User, or Priority.
Select Sorting: Once grouped, tickets can be sorted by Priority (highest first) or Title (alphabetically).
Retain View Settings: When the page is refreshed, the previously selected grouping and sorting options are restored.
Customization Options
UI Enhancements: The look and feel of the Kanban board can be customized by changing the CSS for colors, fonts, and layout styles.
Ticket Fields: You can extend the ticket card component to show more details from the API, based on your requirements.
State Management: For larger-scale applications, integrating a state management tool like Redux can help manage the app's state more efficiently.
Technologies Used
React: For building the user interface.
Axios: For making HTTP requests to the API.
LocalStorage: To store and retrieve the user’s view preferences.
CSS/SCSS: For styling the Kanban board to match any design specifications.