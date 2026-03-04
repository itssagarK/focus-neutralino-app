Focus — Minimal Desktop Focus Timer
Overview

Focus is a lightweight desktop productivity application built using Neutralinojs, HTML, CSS, and JavaScript.

The purpose of this application is to help developers and students stay focused while working on a specific task. The application provides a simple timer that allows users to start a focus session, complete their work, and automatically record the session.

Unlike many productivity tools that contain many complex features and settings, Focus is designed to be minimal and easy to use. The interface only includes the essential tools needed to start working quickly without distractions.

The application also records session history, including the date, time, and duration of each completed focus session.

Why This Project Was Built

Many productivity and timer applications available today contain too many features, dashboards, and settings. While these features may be useful in some cases, they can also make the application complicated and distracting.

The main goal of Focus is to create a simple and distraction-free focus timer.

The idea behind the application is very simple:

start a timer

work on one task

finish the session

automatically save the session history

This helps users stay focused and also track their productivity over time.

The project was also built to demonstrate how web technologies can be used to build lightweight desktop applications using Neutralinojs, instead of heavier frameworks like Electron.

Application Preview

Below is a preview of the Focus desktop application interface.

The interface displays the active timer, the current task input, and the history of completed focus sessions.

Main Features
Focus Timer

The application includes a focus timer that allows users to start a work session.
The timer counts down from the selected number of minutes.

Minimal Interface

The design is intentionally simple and distraction-free so users can quickly start working without unnecessary options or settings.

Session History

Every completed focus session is automatically saved and displayed in the Focus Sessions section.

Date and Time Recording

Each saved session contains:

the date of the session

the time when the session finished

the duration of the focus session

Desktop Notifications

When a focus session ends, the application shows a native desktop notification.

Alarm Sound

An alarm sound plays when the timer reaches zero to inform the user that the session has finished.

System Monitoring

The application can display RAM usage of the system using Neutralinojs native APIs.
This demonstrates interaction between the application and the operating system.

Technologies Used

This project uses the following technologies.

Neutralinojs

Neutralinojs is a lightweight framework used to build cross-platform desktop applications using web technologies.

Unlike Electron, Neutralinojs does not bundle Chromium or Node.js, which makes applications smaller and faster.

HTML

HTML is used to create the structure of the application interface.

CSS

CSS is used to design the layout and appearance of the application.

JavaScript

JavaScript is used to implement the main application logic including:

timer functionality

session storage

session history display

system monitoring

Neutralinojs APIs Used

The project demonstrates several native APIs provided by Neutralinojs.

Filesystem API

Used to store focus session history locally.

Functions used:

Neutralino.filesystem.readFile()
Neutralino.filesystem.writeFile()
Window API

Used to update the application window title dynamically while the timer is running.

Neutralino.window.setTitle()
OS API

Used to show native desktop notifications.

Neutralino.os.showNotification()
Computer API

Used to monitor system memory usage.

Neutralino.computer.getMemoryInfo()
How the Application Works (Step-by-Step)
Step 1 — Launch the Application

When the application starts:

Neutralino initializes the desktop environment

the default timer value appears (25 minutes)

previous session history is loaded from storage

system monitoring begins

Step 2 — Enter Current Task

The user enters the task they want to focus on.

Example:

Complete GSoC proposal

This helps the user stay focused on one specific task.

Step 3 — Start the Focus Session

When the Start Session button is clicked:

the timer starts counting down

the status changes to Focusing

the window title updates with the remaining time

Example window title:

Focus: 24:59
Step 4 — Timer Countdown

Every second:

the timer decreases

the timer display updates

the window title updates

This continues until the timer reaches zero.

Step 5 — Session Completion

When the timer reaches 00:00:

an alarm sound plays

a desktop notification appears

the focus session is automatically saved

Step 6 — Saving Session Data

Session data is stored in a local file called:

sessions.json

Each session record contains:

session ID

timestamp

session duration

Example record:

{
"id": 1741093402,
"timestamp": "4/3/2026, 11:13 PM",
"duration": 25
}
Step 7 — Viewing Session History

The Focus Sessions section displays previously completed sessions.

Users can see:

when the session was completed

how long the session lasted

the total number of sessions completed

Step 8 — Reset Timer

The Reset button stops the current timer and resets it to the selected duration.

Project Structure

Example project folder structure:

focus-app
│
├── index.html
├── styles.css
├── alarm.mp3
├── README.md
│
├── js
│   ├── main.js
│   └── neutralino.js
│
└── screenshots
    └── focus-app.png
How to Run the Project
Install Neutralino CLI
npm install -g @neutralinojs/neu
Run the Application

Navigate to the project folder and run:

neu run

This will launch the desktop application.

Future Improvements

Possible improvements for this project include:

dark mode support

break timer between sessions

productivity analytics dashboard

exporting session history to CSV

system tray integration

keyboard shortcuts

Learning Outcomes

This project helped demonstrate:

building desktop applications using web technologies

using Neutralinojs native APIs

storing data locally using the filesystem API

interacting with system resources

designing a minimal and functional user interface

![image alt]([image_url](https://github.com/itssagarK/focus-neutralino-app/blob/main/focus-app.png.png?raw=true))
