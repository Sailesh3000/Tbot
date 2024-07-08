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

# Setting up Google API Credentials

To integrate with Google Calendar and use the Google Calendar API in this project, you'll need to set up API credentials. Follow these steps:

1. **Create a Project on Google Cloud Console:**
   - Go to the [Google Cloud Console](https://console.cloud.google.com/).
   - Create a new project or select an existing one.

2. **Enable the Google Calendar API:**
   - In the Cloud Console, navigate to the [API Library](https://console.cloud.google.com/apis/library).
   - Search for "Google Calendar API" and enable it for your project.

3. **Set Up OAuth Consent Screen:**
   - In the Cloud Console, navigate to the [OAuth consent screen](https://console.cloud.google.com/apis/credentials/consent).
   - Choose "External" or "Internal" depending on your use case and fill in the required fields like application name, user support email, etc.

4. **Create OAuth Client ID:**
   - In the Cloud Console, navigate to the [Credentials](https://console.cloud.google.com/apis/credentials) section.
   - Click on "Create Credentials" and select "OAuth client ID".
   - Choose "Desktop App" as the application type.
   - Download the `credentials.json` file and save it in the root directory of your project.

5. **Use `credentials.json` in Your Project:**
   - Make sure `credentials.json` is in the same directory as your Python scripts (`timeManager.py`).
   - The script will automatically use this file to authenticate and authorize access to the Google Calendar API.

6. **Run the Project:**
   - Now you can run your Python script (`timeManager.py`).
   - On the first run, it will prompt you to authorize access via a web browser.
   - Follow the provided URL, authorize the application, and copy the authorization code back into the terminal.

By following these steps, you'll be able to successfully set up Google API credentials for your project and integrate with Google Calendar API for time management and event scheduling functionalities.

If you encounter any issues, refer to the [Google Calendar API documentation](https://developers.google.com/calendar) for troubleshooting or additional setup instructions.
