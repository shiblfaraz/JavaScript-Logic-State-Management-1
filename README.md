# JavaScript Logic & State Management – To-Do List

## 📌 Project Overview

This project is a fully functional **To-Do List Web Application** developed using HTML, CSS, and JavaScript.

The main purpose of this project is to understand and implement **JavaScript logic, DOM manipulation, event handling, CRUD operations, filtering, and browser localStorage**.

The application allows users to add, edit, delete, and manage tasks while automatically saving the data in the browser.

---

## 🎯 Task Objective

The objective of this task is to build an interactive client-side To-Do List application that demonstrates:

* JavaScript DOM manipulation
* Event handling
* CRUD operations
* Dynamic element creation
* Event delegation
* Browser `localStorage`
* State management
* Task filtering

---

## ✨ Features

### 1. Add Tasks

Users can enter a task and add it to the To-Do List.

### 2. Edit Tasks

Existing tasks can be edited and updated.

### 3. Delete Tasks

Users can remove tasks from the list.

### 4. Mark Tasks as Completed

Users can mark a task as completed or active.

### 5. Task Filters

The application provides three filters:

* **All** – Displays all tasks
* **Active** – Displays only incomplete tasks
* **Completed** – Displays completed tasks

### 6. Local Storage

Tasks are automatically stored using:

```javascript
window.localStorage
```

This allows tasks to remain available even after refreshing or reopening the browser.

### 7. Dynamic DOM Manipulation

Task elements are dynamically created and updated using JavaScript instead of manually adding every task in HTML.

### 8. Event Delegation

Event delegation is used to efficiently handle interactions with dynamically created task elements.

---

## 🛠️ Technologies Used

* **HTML5**
* **CSS3**
* **JavaScript**
* **DOM API**
* **Browser Local Storage**

---

## 📂 Project Structure

```text
todo-list/
│
├── index.html
├── style.css
├── script.js
└── README.md
```

---

## ⚙️ How It Works

### Step 1 – User Adds a Task

The user enters a task in the input field and clicks the **Add** button.

### Step 2 – JavaScript Creates the Task

JavaScript creates a task object and dynamically adds it to the task list.

Example:

```javascript
{
    id: 1,
    text: "Complete JavaScript task",
    completed: false
}
```

### Step 3 – State is Updated

The application maintains the current list of tasks in JavaScript.

### Step 4 – Data is Saved

The task data is converted into JSON and stored in `localStorage`.

```javascript
localStorage.setItem("tasks", JSON.stringify(tasks));
```

### Step 5 – Tasks are Restored

When the page is opened again, the stored tasks are retrieved.

```javascript
const tasks = JSON.parse(localStorage.getItem("tasks")) || [];
```

### Step 6 – Filtering

The application checks the task status and displays the appropriate tasks based on the selected filter.

---

## 🔄 CRUD Operations

The application implements the four basic CRUD operations:

| Operation | Function                |
| --------- | ----------------------- |
| Create    | Add a new task          |
| Read      | Display saved tasks     |
| Update    | Edit or complete a task |
| Delete    | Remove a task           |

---

## 💾 Local Storage

The application uses browser `localStorage` to provide data persistence.

Tasks are converted into a JSON string before storing them:

```javascript
localStorage.setItem("tasks", JSON.stringify(tasks));
```

When the application starts, the stored information is retrieved:

```javascript
const savedTasks = JSON.parse(localStorage.getItem("tasks")) || [];
```

This ensures that the user's tasks are not lost when the page is refreshed.

---

## 🖱️ Event Handling

JavaScript event listeners are used to handle user interactions such as:

* Adding tasks
* Editing tasks
* Deleting tasks
* Completing tasks
* Changing filters

Event delegation is used on the task container so that dynamically generated task elements can also respond to user actions.

---

## 🚀 How to Run the Project

### Method 1 – Open Directly

1. Download or clone the project.
2. Open the project folder.
3. Double-click `index.html`.
4. The To-Do List will open in the browser.

### Method 2 – Using VS Code

1. Open the project in **Visual Studio Code**.
2. Open `index.html`.
3. Install the **Live Server** extension if required.
4. Right-click `index.html`.
5. Select **Open with Live Server**.
6. The application will open in the browser.

---

## 🧪 Testing

The following functionality was tested:

* [x] Add a new task
* [x] Display tasks dynamically
* [x] Edit a task
* [x] Delete a task
* [x] Mark task as completed
* [x] Display all tasks
* [x] Display active tasks
* [x] Display completed tasks
* [x] Save tasks to localStorage
* [x] Restore tasks after page refresh
* [x] Handle dynamically created task elements

---

## 📚 Concepts Learned

Through this project, the following JavaScript concepts were practiced:

* Variables and arrays
* Objects
* Functions
* Conditional statements
* Array methods
* DOM manipulation
* Event listeners
* Event delegation
* JSON
* `localStorage`
* State management
* CRUD operations

---

## 🎓 Learning Outcome

After completing this project, I gained practical experience in developing interactive web applications using JavaScript.

The project helped me understand how **JavaScript manages application state, updates the DOM dynamically, handles user interactions, and stores data persistently using localStorage**.

---

## 👨‍💻 Project Information

**Task:** Task 3 – JavaScript Logic & State Management
**Project:** To-Do List Application
**Technologies:** HTML, CSS, JavaScript
**Type:** Client-Side Web Application
