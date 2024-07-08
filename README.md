# Project Summary

This project is a Python-based time management system that integrates with Google Calendar to track coding hours and manage events programmatically. It allows users to:

- Retrieve today's coding hours from Google Calendar and display a summary.
- Add custom events to Google Calendar with specified durations and descriptions.
- Store coding hours in a SQLite database (`hours.db`) for record-keeping and analysis.

The system uses the Google Calendar API for interacting with calendar events and utilizes SQLite for local data storage. It provides a straightforward way to automate time tracking and event management tasks, enhancing productivity and organization for coding and related activities.

## Prerequisites

Before running this project, make sure you have the following installed:

- Python 3.x
- `pip` package manager
- Google Calendar API credentials (`credentials.json`)
- SQLite database engine (included with Python standard library)

## Setup

1. **Clone the repository:**

   ```bash
   git clone <repository-url>
   cd <repository-directory>
