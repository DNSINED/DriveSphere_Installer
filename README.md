# Send Via GDrive (DriveSphere)

## Overview

This project requires access to Google Drive API for its functionality. Below are the steps to create a Google Cloud Console account, enable the Google Drive API, create a service account with the owner role, generate a key, and prepare the configuration file. Additionally, you will need to set up Python and install the required dependencies.

## Prerequisites

- A Google account
- Basic understanding of Google Cloud Console
- Python installed on your system
- pip (Python package installer)

## Steps to Setup Google Drive API Access

### 1. Create a Google Cloud Console Account

1. Visit the [Google Cloud Console](https://console.cloud.google.com/).
2. Sign in with your Google account.
3. If you don't have a project already, click on the **Select a project** dropdown at the top and select **New Project**.
4. Enter the project name and click **Create**.

### 2. Enable Google Drive API

1. In the Google Cloud Console, navigate to **APIs & Services** > **Library**.
2. Search for "Google Drive API".
3. Click on **Google Drive API**.
4. Click the **Enable** button.

### 3. Create a Service Account

1. Go to **IAM & Admin** > **Service Accounts**.
2. Click on the **+ CREATE SERVICE ACCOUNT** button.
3. Enter a service account name and description.
4. Click **Create and Continue**.
5. In the **Select a role** dropdown, choose **Owner**.
6. Click **Continue**, then **Done**.

### 4. Generate a Key for the Service Account

1. In the **Service Accounts** page, locate the newly created service account.
2. Under the **Actions** column, click on the three dots (⋮).
3. Select **Manage keys**.
4. Click on **Add Key** > **Create new key**.
5. Ensure **JSON** is selected and click **Create**.
6. The key file will be downloaded automatically. Save this file.

### 5. Prepare the Configuration File

1. Locate the downloaded JSON key file.
2. Rename the file to `config_gdrive.json`.
3. Move this file to the installation directory of your project.

## Setting Up the Development Environment

### 1. Install Python

1. Download the latest version of Python from the [official Python website](https://www.python.org/).
2. Run the installer and ensure you check the box that says **Add Python to PATH**.
3. Follow the prompts to complete the installation.

### 2. Verify Python Installation

1. Open a terminal (Command Prompt on Windows, Terminal on macOS/Linux).
2. Type `python --version` and press Enter. You should see the installed Python version.

### 3. Install pip

1. Pip is typically installed with Python. To verify, type `pip --version` in the terminal and press Enter.
2. If pip is not installed, follow the instructions on the [pip installation page](https://pip.pypa.io/en/stable/installation/).

### 4. Install Required Python Packages

1. Open a terminal.
2. Navigate to the project directory.
3. Run the following command to install the Google API Python client:
   ```sh
   pip install google-api-python-client
   ```
## Running the Project

1. Ensure that the `config_gdrive.json` file is in the correct directory.
2. Follow any additional project-specific setup instructions provided in the project documentation.

## Troubleshooting

- If you encounter any issues, refer to the [Google Cloud Documentation](https://cloud.google.com/docs) for further assistance.
- Ensure you have the necessary permissions and roles assigned in the Google Cloud Console.
- Verify that Python and pip are correctly installed and added to the system PATH.

## Contact

For further questions or support, contact [sendviagdrive@gmail.com].
