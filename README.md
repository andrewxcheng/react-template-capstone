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

### 5. Install Dependencies
Inside the terminal, you'll need to install the template on your computer.

Type the following into your terminal:
`npm install`

This installs React, Vite, and all required packages. These are the dependencies that your project runs on.

You only need to do this once throughout the lifespan of your project (or whenever dependencies change).

### 6. Start the Development Server

To start your web application, run the following on your terminal:
`npm run dev`

You should see output similar to:

VITE vX.X.X  ready in XXX ms
➜  Local:   http://localhost:5173/

You can then open the URL in your browser to see your application. To close the server, use Ctrl+C in the terminal.

Congratulations, your web application is now running!

## Making Changes to Your Application
JSX allows you to write HTML-like code inside JavaScript. Here, the code simply creates a page with a greeting in a heading.

Example (src/App.jsx):
```
function App() {
  return (
    <div>
      <h1>Hello! This is my React+Express Application</h1>
    </div>
  );
}

export default App;
```

The code works as following:
`<div>` 
* A `<div>` is a container element
* It groups content together on the page

`<h1>`
* `<h1>` is a heading tag. It represents the largest and most important heading on the page
* HTML has heading levels from `<h1>` (largest) to `<h6>` (smallest)
* The text inside the `<h1>` tag is what appears on the screen

Some other elements you may want to include in your application include:

`<img>`
* Displays an image based on a source location
```
<img src="/assets/myImage.png" />
```

`<a>`
* Creates a clickable link
* Uses a property called `href` to define the destination of the link

`<input>`
* Allows users to type in information, such as `text`, `password`, `email`
* Commonly used for forms

`<form>`
* Creates a form for your application
```
<form>
  <input type="text" placeholder="Username" />
  <button type="submit">Submit</button>
</form>
```

To make any changes to your application manually, use the following steps:
* Edit src/App.jsx
* Save the file
* The browser updates automatically

## Coding with Agentic AI
VSCode’s Agent mode can help you go from idea → working code by generating files, editing multiple parts of your project, and fixing errors with you. Now that you have a template, VSCode can easily work to develop features on top of the template. 

### Tell the Agent what you want to build
Open the Agent/Agent Build panel (varies by extension, but usually in the sidebar or command palette).

Give it a clear goal, plus constraints. Example prompt:

“Create an expense management application that has a chat interface for receipts to be uploaded.”

You can also ask a separate LLM to create a prompt, so that features are more specific. Try asking an LLM for a project scaffold to feed into a coding agent, and the LLM will create a framework you can provide VSCode.

### Debug with the Agent
When something breaks, paste the error and ask for a fix. If your app won’t run, copy the exact terminal error and try asking:

“Here’s my error. Explain what it means and give the smallest fix.”

“Fix this without changing the project structure.”

“Show me the exact file + lines to edit.”

## Minimal Project Structure
```
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
```

## Summary
Congratulations, you've now set up your own web app to be built into anything you choose!

In summary,
* Node runs the tooling
* Vite runs a development server
* React renders the user interface 
* JSX is the language of React, which combines HTML and JavaScript
* Edit App.jsx to build your application

Good luck!