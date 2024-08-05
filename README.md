Todo Application
Overview
The Todo Application is a web-based task management tool designed using React. It allows users to add, update, complete, and remove tasks. The application also supports search functionality using URL parameters, enabling users to filter tasks based on a search query. The app uses react-router-dom to handle routing and URL management.

System Design
Frontend Components
TodoList: The main component that manages the list of tasks, search functionality, and integration with other components.
Todo: Displays individual todo items with options to edit, complete, or delete.
TodoForm: A form for adding and updating todo items.
Data Management
State Management: Tasks are managed using React's state (useState).
Data Storage: Data is initially fetched from a data.json file and manipulated within the app.
Search Functionality: Implemented using URL parameters to filter tasks.
Routing
React Router: Used for managing URL parameters and enabling search functionality.
Implementation
Components
TodoList: Manages the overall list of todos, handles search queries from URL parameters, and updates the URL based on user input.
Todo: Displays each todo item and handles interactions such as marking as complete, editing, and deleting.
TodoForm: Provides an input form for adding new todos and updating existing ones.
Search Functionality
Search queries are managed through URL parameters.
Users can search for tasks, and the results are filtered based on the query.
URL parameters update when the search is performed, allowing users to bookmark or share search results.
Data Storage
A dummy data.json file is used as the initial data repository.
Data can be manipulated within the app but is not persisted beyond the current session.
Styling
Basic styles are applied to make the application visually appealing and user-friendly.

URL Parameters
Search: Use the search parameter to filter tasks. For example, http://localhost:3000?search=meeting filters tasks containing "meeting".

Directory Structure
/public
  /data.json
/src
  /components
    Todo.js
    TodoForm.js
    TodoList.js
  App.js
  index.js
/App.css
README.md

Styling: Custom styles are provided in App.css.
Routing: Handled using react-router-dom for URL management and search functionality.
Feel free to modify or extend the application as needed. For any issues or feature requests, please create an issue in the repository.

Deployed Link: https://venom1547.github.io/To-do
