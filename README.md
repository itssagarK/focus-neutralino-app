#  **Focus — Lightweight Desktop Productivity Timer**



**Focus** is a **lightweight desktop productivity application** built using **Neutralinojs, HTML, CSS, and JavaScript**.

The goal of this application is to help **developers and students stay focused on a single task** by providing a **minimal and distraction-free focus timer**.

Unlike many productivity tools that include **complex dashboards and unnecessary features**, **Focus follows a minimal design philosophy**, allowing users to **start working quickly and track their productivity easily**.

---

# 📸 **Application Preview**

![Focus App](https://github.com/itssagarK/focus-neutralino-app/blob/main/focus-app.png.png?raw=true)

The screenshot above shows the **Focus desktop timer during an active focus session**, displaying:

- **Current task input**
- **Live countdown timer**
- **Session history tracking**
- **System resource monitoring**

---

# 🚀 **Key Features**

### ⏱ **Focus Timer**
A **simple and precise countdown timer** designed for productivity sessions.

The timer counts down from the selected number of minutes and updates **every second**.

---

### 🧠 **Minimal Interface**
The application follows a **clean and distraction-free design** so users can start working immediately without complicated settings.

---

### 📜 **Session History**
Every completed session is **automatically saved** and displayed in the **Focus Sessions section**.

---

### 📅 **Date & Time Tracking**
Each session record contains:

- **Session date**
- **Session completion time**
- **Session duration**

This allows users to **track their productivity over time**.

---

### 🔔 **Desktop Notifications**
When a focus session finishes, the application sends a **native desktop notification** using the **Neutralinojs OS API**.

---

### 🔊 **Alarm Sound**
An **alarm sound** plays when the timer reaches **zero**, notifying the user that the focus session has ended.

---

### 💻 **System Resource Monitoring**
The application can display **RAM usage of the system** using the **Neutralinojs Computer API**, demonstrating **interaction between the application and the operating system**.

---

# 🎯 **Why This Project Was Built**

Many productivity applications today contain **too many features, dashboards, and configuration options**, which often make them **complicated and distracting**.

The goal of **Focus** is to provide a **simple productivity tool** that helps users stay focused on a single task.

The workflow is intentionally simple:

1. **Start a timer**
2. **Work on one task**
3. **Complete the session**
4. **Automatically save the session history**

This approach helps users **stay productive while keeping the application lightweight and easy to use**.

The project also demonstrates how **modern web technologies can be used to build lightweight desktop applications using Neutralinojs instead of heavier frameworks like Electron**.

---

# 🛠 **Technologies Used**

| Technology | Purpose |
|------------|--------|
| **Neutralinojs** | Lightweight desktop application framework |
| **HTML** | Application structure |
| **CSS** | User interface styling |
| **JavaScript** | Application logic |

---

# ⚙ **Neutralinojs APIs Used**

The project demonstrates several **native APIs provided by Neutralinojs**.

| API Module | Purpose |
|-----------|--------|
| **Neutralino.filesystem** | Read and write session history (`sessions.json`) |
| **Neutralino.os** | Display native desktop notifications |
| **Neutralino.window** | Update window title dynamically |
| **Neutralino.computer** | Monitor system RAM usage |

Example API usage:

```javascript
Neutralino.filesystem.readFile()
Neutralino.filesystem.writeFile()
Neutralino.window.setTitle()
Neutralino.os.showNotification()
Neutralino.computer.getMemoryInfo()
