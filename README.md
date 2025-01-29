# Task Manager

A simple and intuitive Task Manager application built with React. This app allows users to create, view, mark tasks as complete/incomplete, and delete tasks. It demonstrates a strong understanding of React concepts such as component composition, state management, and event handling.

## Overview
<img width="1180" alt="Screenshot 2025-01-29 at 2 31 51 pm" src="https://github.com/user-attachments/assets/17a3d3fc-1c17-43b6-b213-e142b58dcef0" />

### Explanation:
#### 1. App.jsx (Main Application)
- Holds the state (`tasks` array).
- Handles adding, deleting, and completing tasks.
- Passes tasks to `TaskList` and `TaskForm`.

#### 2. TaskForm.jsx
- Contains an input field and a submit button.
- Calls `addTask` function in `App.jsx` when a new task is added.

#### 3. TaskList.jsx
- Receives `tasks` from `App.jsx` and renders each one using `TaskItem.jsx`.

#### 4. TaskItem.jsx
- Displays a single task with "Complete" and "Delete" buttons.
- Calls functions to toggle completion status and delete a task.

### Data Flows:
1. User enters a task → `TaskForm.jsx` calls `addTask()`.
2. `addTask()` updates the state in App.jsx.
3. Updated state is passed to `TaskList.jsx`, which re-renders the task list.
4. Each task is displayed using `TaskItem.jsx`.
5. Clicking "Complete" or "Delete" triggers state updates in `App.jsx`, and the UI updates accordingly.

## Features
- **Add Tasks**: Create new tasks using a simple form.
- **View Tasks**: Display a list of tasks with their current status.
- **Mark as Complete**: Toggle tasks between completed and incomplete states with visual strikethrough.
- **Delete Tasks**: Remove tasks from the list.
- **Dynamic UI**: Responsive updates to the task list using React's state management.

## Technologies Used

- **React**: Frontend library for building the user interface.
- **Vite**: Fast and modern development build tool.
- **CSS**: For styling the application.
- **Node.js and npm**: To manage dependencies and run the project.


## Installation and Setup - Method 01

Follow these steps to run the project locally:

### 1. Clone the repository:
```
git clone https://github.com/MenakaGodakanda/task-manager.git
cd task-manager
```

### 2. Install dependencies:
```
npm install
```

### 3. Start the development server:
```
npm run dev
```

### 4. Open your browser and navigate to:
```
http://localhost:5173
```

## Installation and Setup - Method 02

### 1. Install Node.js and npm
- React requires `Node.js` and `npm` (Node Package Manager) to manage dependencies.
- Open your terminal and run:
```
sudo apt update
sudo apt install -y nodejs npm
```

- Verify the installations:
```
node -v
npm -v
```

- Install the latest version of Node.js:
```
sudo npm install -g n
sudo n stable
```
![Screenshot 2025-01-15 034830](https://github.com/user-attachments/assets/b15a0d55-b1a3-4ec8-857a-97805530b4cd)

### 2. Set Up Your React Project
- Create a new React application using Vite, a faster alternative to Create React App:
```
npm create vite@latest task-manager -- --template react
cd task-manager
```
![Screenshot 2025-01-15 034943](https://github.com/user-attachments/assets/a846f130-7d39-4277-a268-df6d204092ff)

- Install dependencies:
```
npm install
```
![Screenshot 2025-01-15 035058](https://github.com/user-attachments/assets/b40247e0-c55b-4f06-ae87-219f665baf10)

- Open the project in your preferred text editor, e.g., Visual Studio Code:
```
code .
```

### 3. Develop the Application
- Follow the file structure and create and modify below files.
- Modify the `App.jsx`
- Create the `TaskForm.jsx`
- Create the `TaskList.jsx`
- Create the `TaskItem.jsx`
- Open `src/index.css` and add some basic styles.

### 4. Run the Application
- Start the development server:
```
npm run dev
```
![Screenshot 2025-01-15 035727](https://github.com/user-attachments/assets/4fa40ccf-17fd-4de2-bc7a-a3fa3bf9d897)

- Open your browser and navigate to `http://localhost:5173`.

## Screenshots

### 1. Initial View
- The user sees the app title, an input field, and a button to add tasks.
![Screenshot 2025-01-15 035745](https://github.com/user-attachments/assets/b8f7b4e1-0d71-46e1-a5b5-d59c80ca9c81)


### 2. After Adding Tasks
- The task appears in the list below, with two buttons:
  - **Complete**: Marks the task as completed.
  - **Delete**: Removes the task from the list.
- If you click "Add Task" without typing anything, nothing happens because of validation in the `TaskForm` component.
![Screenshot 2025-01-15 035825](https://github.com/user-attachments/assets/0dc900dc-9d35-43dd-bafe-5679ffec338d)

### 3. After Marking a Task as Complete
- The task text will be styled with a strikethrough to indicate completion (e.g., Complete React project).
- The button text changes to "Undo". Clicking "Undo" will remove the strikethrough and revert the task to its incomplete state.
![Screenshot 2025-01-15 035849](https://github.com/user-attachments/assets/ec3b3c06-30e4-42cd-8fd1-00204e6a6fc7)
![Screenshot 2025-01-15 040012](https://github.com/user-attachments/assets/69c659ae-b9a2-4a1c-8ab9-f95e0bada953)



### 4. After Deleting a Task
- The task is removed from the list immediately.
![Screenshot 2025-01-15 040031](https://github.com/user-attachments/assets/5654355f-c0be-4478-9848-750ede1d18d8)


## Project Structure
```
task-manager/
├── index.html      # Entry HTML file
├── src/
│   ├── components/
│   │   ├── TaskForm.jsx   # Component for adding tasks
│   │   ├── TaskList.jsx   # Component for displaying tasks
│   │   └── TaskItem.jsx   # Component for individual tasks
│   ├── App.jsx            # Main application component
│   ├── index.css          # Application styles
│   └── main.jsx           # React entry point
├── package.json           # Project dependencies
├── vite.config.js         # Vite configuration
└── README.md              # Project documentation
```

## License

This project is licensed under the MIT License.
