# ⏰ Event Reminder

> **Smart event management made simple.** A Java-based desktop application that helps you track, manage, and get reminded about important events with an intuitive GUI and persistent storage.

[![Java](https://img.shields.io/badge/Java-11%2B-orange)](https://www.java.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Active-brightgreen.svg)](#)

---

## ✨ Features

### Core Functionality
- ✅ **Add Events** - Create events with name and date/time
- 🔔 **Automatic Reminders** - Get notified of events within the next 24 hours
- 💾 **Persistent Storage** - Save events to file for data persistence
- 📋 **Event List** - View all your events in a clean table format
- 🗑️ **Delete Events** - Remove events you no longer need
- 🕐 **DateTime Formatting** - Easy-to-read date and time format (dd-MM-yyyy HHmm)

### User Interface
- 🎨 **Swing GUI** - Modern graphical interface
- 📊 **Event Table** - Display all events in a table with sorting
- 🖱️ **Easy Navigation** - Simple buttons for adding and deleting events
- 💬 **Dialog Boxes** - Input events with user-friendly dialogs

---

## 🛠️ Tech Stack

| Component | Technology |
|-----------|------------|
| **Language** | Java 11+ |
| **GUI Framework** | Swing (javax.swing) |
| **Data Storage** | Text File (events.txt) |
| **Date/Time** | Java LocalDateTime |
| **Build Tool** | (Optional) Maven/Gradle |

---

## 🚀 Quick Start

### Prerequisites
- Java 11 or higher installed
- JDK (Java Development Kit)

### Installation

1. **Clone the repository:**
```bash
git clone https://github.com/Eswarpulavarthi/Event-Reminder.git
cd Event-Reminder
```

2. **Compile the Java files:**
```bash
javac Event.java
javac EventManager.java
javac EventReminderGUI.java
```

3. **Run the application:**
```bash
java EventReminderGUI
```

---

## 📖 Usage Guide

### Adding an Event
1. Click the **"Add Event"** button
2. Enter the event name when prompted
3. Enter the date and time in format: `dd-MM-yyyy HHmm`
   - Example: `25-12-2025 1800` (6 PM on Dec 25, 2025)
4. The event appears in the table

### Viewing Events
- All events are displayed in the table with name and date/time
- Events are loaded automatically from `events.txt` on startup

### Deleting an Event
1. Select an event from the table
2. Click the **"Delete Event"** button
3. The event is removed from the list and file

### Getting Reminders
- On startup, the application checks for events within the next 24 hours
- A dialog box appears showing upcoming reminders
- Reminders use the format: `Event Name - dd-MM-yyyy HHmm`

---

## 📁 Project Structure

```
Event-Reminder/
├── Event.java                 # Event data model
├── EventManager.java          # Business logic for events
├── EventReminderGUI.java      # Swing GUI implementation
├── events.txt                 # Data persistence file (auto-generated)
├── README.md
├── .gitignore
└── LICENSE
```

---

## 🏗️ Architecture

### Class Hierarchy

**Event.java**
- Represents a single event
- Properties: name, dateTime
- Provides getters and toString()

**EventManager.java**
- Manages collection of events
- Handles file I/O (loadEventsFromFile, saveAllEventsToFile)
- Provides CRUD operations (add, delete, get)
- Filters upcoming events within 24 hours

**EventReminderGUI.java**
- Extends JFrame
- Creates the main window with table and buttons
- Handles user interactions (add, delete)
- Displays reminders on startup
- Updates table after each operation

### Data Flow
```
GUI Input → EventManager → File Storage
  ↓
Load File → EventManager → GUI Display
```

---

## 🎯 Learning Outcomes

This project demonstrates:
- **Object-Oriented Programming** (classes, inheritance, encapsulation)
- **GUI Development** using Swing framework
- **File I/O** operations in Java
- **Date/Time Handling** with LocalDateTime
- **Event-Driven Programming** (ActionListeners)
- **Data Persistence** and model management
- **MVC Architecture** (Model-View-Controller pattern)

---

## 💡 Future Enhancements

- [ ] **Database Integration** - Replace file storage with SQLite/MySQL
- [ ] **Recurring Events** - Support daily, weekly, monthly reminders
- [ ] **Categories** - Organize events by type (work, personal, etc.)
- [ ] **Notifications** - System tray notifications and sound alerts
- [ ] **Import/Export** - CSV or ICS file support
- [ ] **Search & Filter** - Find events by name or date range
- [ ] **Dark Mode** - Modern UI theme
- [ ] **Web Version** - Java web framework (Spring Boot)

---

## 📝 Sample Data Format

The `events.txt` file stores events in this format:
```
Meeting with team|25-12-2025 1400
Doctor appointment|26-12-2025 1000
Project deadline|31-12-2025 2359
```

---

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add improvement'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙌 Support & Feedback

- 🐛 Found a bug? [Open an issue](https://github.com/Eswarpulavarthi/Event-Reminder/issues)
- 💡 Have an idea? [Start a discussion](https://github.com/Eswarpulavarthi/Event-Reminder/discussions)
- ⭐ Like this project? Please star it!

---

## 👨‍💻 Author

**Eswarpulavarthi**
- GitHub: [@Eswarpulavarthi](https://github.com/Eswarpulavarthi)
- Portfolio-building project for Java and GUI development practice

---

**Last updated:** December 2025
