# 📝 Asynchronous Logger System

This project implements a high-performance **Asynchronous Logger** in Python, tailored for multi-threaded environments. It ensures non-blocking logging, efficient log rotation, and thread safety while maintaining application performance.

---

## 🚀 Features

- **Singleton Design Pattern**: Guarantees a single instance of the logger throughout the application lifecycle.
- **Thread-Safe Logging**: Allows concurrent log message writing without conflicts or data races.
- **Asynchronous Logging**: Uses a background thread to handle logging separately from the main application logic.
- **Log Rotation**: Automatically creates a new log file when the current one exceeds a defined size limit.
- **Graceful Shutdown**: Ensures that all pending log messages are written before termination.

---

## ⚙️ Tech Stack

- **Language**: Python
- **Concepts**: Multithreading, File Handling, Design Patterns
- **Tools**: `queue`, `threading`, `os`, `time`, `logging`

---

## 📁 Project Structure

```bash
logger_system/
├── logger.py              # Core asynchronous logger implementation
├── app.py                 # Example usage of the logger in a multi-threaded environment
├── logs/                  # Rotating log files are saved here
└── README.md              # Project documentation
