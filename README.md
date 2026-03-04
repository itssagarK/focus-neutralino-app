Focus — Minimal Desktop Focus Timer
Project Overview
Focus is a lightweight desktop productivity application built using Neutralinojs, HTML, CSS, and JavaScript.
The goal of this application is to help developers and students stay focused while working on a task. The app provides a simple timer that allows users to work in focused sessions and track their completed work sessions.
Unlike many productivity tools that include too many features, Focus is intentionally minimal and easy to use. The interface only contains the essential tools needed to start a focus session and track productivity.
The application also records session history, including the date, time, and duration of each focus session.

Why This Project Was Built
Many productivity applications are complicated and contain too many features. These extra features can sometimes make the app harder to use and distract users from their work.
This project was built to create a simple and distraction-free focus timer.

The main idea behind Focus is:
start a timer
work on a single task
save the session automatically
track your productivity history

The application is designed to be minimal, lightweight, and fast, making it easy for anyone to start focusing on their work without unnecessary complexity.
Main Features
Focus Timer
Users can start a focus session using a timer. The timer counts down from the selected number of minutes.
Session History
Every completed session is automatically saved and displayed in the Focus Sessions section.
Date and Time Recording

Each session record contains:
the date
the time
the session duration
Desktop Notification
When a focus session finishes, the app shows a desktop notification to inform the user.
Alarm Sound
An alarm sound plays when the timer reaches zero.
System Monitoring
The application can display the RAM usage of the system using Neutralinojs native APIs.

Technologies Used
This project is built using the following technologies:
Neutralinojs
A lightweight framework used to build desktop applications using web technologies.
HTML
Used to create the structure of the application interface.
CSS
Used to design the layout and appearance of the application.
JavaScript
Used to control the application logic, including the timer, session storage, and system monitoring.
Neutralinojs APIs Used
The application demonstrates several Neutralinojs native APIs:

Filesystem API
Used to store session history locally.
Functions used:
Neutralino.filesystem.readFile()
Neutralino.filesystem.writeFile()
Window API
Used to update the application window title with the remaining timer.
Function used:
Neutralino.window.setTitle()
OS API
Used to display desktop notifications.

Function used:
Neutralino.os.showNotification()
Computer API
Used to monitor system memory usage.
Function used:
Neutralino.computer.getMemoryInfo()



Application Interface:
The screenshot below shows the Focus desktop application running a focus session.

The interface displays the active timer, the current task, and the recorded focus session history.  
When the timer finishes, the session is automatically saved with the date, time, and session duration.

![Focus App Screenshot](screenshot.png)
Focus is a minimal desktop focus timer built using Neutralinojs.

The application helps users stay productive by allowing them to run focus sessions and track completed work sessions with timestamps.
