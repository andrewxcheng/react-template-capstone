# Minimal React + Vite Template

This repository is an extremely minimal setup for building a web application using React.
It is designed for beginners or anyone who wants a clean starting point.

This guide walks you from zero → writing JSX, assuming no prior setup.

## Installation Guide
### 1. Install Prerequisites
#### Node.js (Required)
Node.js is a tool that lets computers run JavaScript programs outside of a web browser. Normally, JavaScript only works on websites to make pages interactive, but Node.js allows it to run on a server instead (in this case, using your computer as a server), where it can handle things like saving data, responding to user requests, or powering an app behind the scenes.

Node.js includes npm, which Vite uses to run and build your app.

1. Go to https://nodejs.org
2. Download the LTS (Long Term Support) version
3. Run the installer and accept all defaults

#### Install Visual Studio Code (Recommended)
Visual Studio Code (often called VS Code) is a free program that developers use to write and edit code. It works like a very powerful text editor, but with helpful features that make coding easier, such as highlighting mistakes, suggesting code as you type, and organizing files in a project.

1. Download: https://code.visualstudio.com
2. Install with default settings

### 2. Download the Project from GitHub
Now, you're ready to download and open the template on your computer. The simplest way to do this is to download this repository as a ZIP file and extract it onto your computer.

1. Click the green Code button on GitHub
2. Select Download ZIP
3. Extract the folder to a convenient location (e.g. Documents/Projects)

### 3. Open the Project in VS Code
Next you'll want to open the code to begin editing it.

1. Open VS Code
2. Click File → Open Folder
3. Select the project folder

### 4. Open a Windows Terminal
After opening a template in VS Code, you need to open a Windows terminal because VS Code is mainly for writing and viewing files, while the terminal is used to run commands that make the project actually work.

To open a terminal:
* Click Terminal → New Terminal

To open the terminal with shortcuts:
* Windows/Linux: `Ctrl + ``
* Mac: `Cmd + ``

### 5. Install Dependencies
Inside the terminal, you'll need to install the template on your computer. Type the following into your terminal:
`npm install`

This installs React, Vite, and all required packages. These are the dependencies that your project runs on.

You only need to do this once throughout the lifespan of your project (or whenever dependencies change).

### 6. Start the Development Server

To start your web application, run the following on your terminal:
`npm run dev`

You should see output similar to:

VITE vX.X.X  ready in XXX ms
➜  Local:   http://localhost:5173/

You can then open the URL in your browser to see your application.

Congratulations, your web application is now running!

## Minimal Project Structure
.
├── node_modules/
├── index.html
├── package.json
├── package-lock.json
├── vite.config.js
├── .gitignore
└── src/
    ├── main.jsx
    └── App.jsx
    ├── index.css
    └── App.css


## File overview
### node_modules

### index.html
The single HTML file. React mounts into this file.

### package.json, package-lock.json

### vite.config.js

### .gitignore

### main.jsx and App.jsx
The entry point that connects React to the DOM.
The main React component where you write JSX.

### index.css and App.css

## JSX Programming

JSX allows you to write HTML-like code inside JavaScript.

Example (src/App.jsx):

function App() {
  return (
    <div>
      <h1>Hello, world</h1>
      <p>This is JSX</p>
    </div>
  );
}

export default App;

## Making Changes

Edit src/App.jsx

Save the file

The browser updates automatically

No manual refresh required.

### Adding a New Component

Create a new file:

src/Hello.jsx

function Hello() {
  return <h2>Hello from another component</h2>;
}

export default Hello;


Import and use it in App.jsx:

import Hello from "./Hello";

function App() {
  return (
    <div>
      <Hello />
    </div>
  );
}

## Coding with Agentic AI


## Stopping the Server

To stop the development server: Ctrl + C

## Summary
Congratulations, you've now set up your own web app to be built into anything you choose!

In summary,
* Node runs the tooling
* Vite runs a development server
* React renders the user interface 
* JSX is the language of React, which combines HTML and JavaScript
* Edit App.jsx to build your application

Good luck!