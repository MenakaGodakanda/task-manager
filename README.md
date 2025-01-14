# Task Manager

A simple and intuitive Task Manager application built with React. This app allows users to create, view, mark tasks as complete/incomplete, and delete tasks. It demonstrates a strong understanding of React concepts such as component composition, state management, and event handling.

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

### 2. Set Up Your React Project
- Create a new React application using Vite, a faster alternative to Create React App:
```
npm create vite@latest task-manager -- --template react
cd task-manager
```

- Install dependencies:
```
npm install
```

- Open the project in your preferred text editor, e.g., Visual Studio Code:
```
code .
```

### 3. Develop the Application
- Follow the file structure
- Modify the `App.jsx`
- Create the `TaskForm.jsx`
- Create the `TaskList.jsx`
- Create the `TaskItem.jsx`
- Open `src/index.css` and add some basic styles:

### 4. Run the Application
- Start the development server:
```
npm run dev
```
- Open your browser and navigate to `http://localhost:5173`.

## Screenshots

### 1. Initial View
- The user sees the app title, an input field, and a button to add tasks.

### 2. Adding and Completing Tasks
- Tasks are displayed in a list with options to complete or delete them.

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
