TODO-APP

A simple and clean Todo List Application built using
Node.js, Express.js, PostgreSQL, HTML, CSS, and EJS templating.
This app allows users to add, edit, and delete tasks with full database integration.


Features

✔ Add new todo items
✔ Edit existing tasks
✔ Delete tasks
✔ Stores todos permanently in PostgreSQL database
✔ EJS templating for server-side rendering
✔ Clean and responsive UI
✔ Organized project structure

Tech Stack

Layer	                 Technology
Backend	               Node.js, Express.js
Database	             PostgreSQL
View Engine	           EJS
Frontend	             HTML, CSS, JS
Styling	               Custom CSS
Version Control        Git / GitHub


Project Structure

todo-app/
│── public/
│── views/
│   ├── index.ejs
│── index.js
│── package.json
│── package-lock.json
│── .gitignore

Installation & Setup

1. Clone the repository
git clone https://github.com/KUMAR0DEEPAK/todo-app.git
cd todo-app

2. Install dependencies
npm install

3. Setup PostgreSQL

Create a PostgreSQL database:

CREATE DATABASE permalist;


Then create the table:

CREATE TABLE items (
  id SERIAL PRIMARY KEY,
  title VARCHAR(255)
);


Update your index.js PostgreSQL credentials if needed:

const db = new pg.Client({
  user: "postgres",
  host: "localhost",
  database: "permalist",
  password: "YOUR_PASSWORD",
  port: 5432
});

4. Start the server
node index.js


Server runs at:

👉 http://localhost:3000

ScreenShot


<img width="1690" height="928" alt="Screenshot (60)" src="https://github.com/user-attachments/assets/157b2909-6a8d-4552-9968-f4be9ac7211f" />



