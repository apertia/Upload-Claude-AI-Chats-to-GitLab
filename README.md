# Upload Claude AI Chats to Gitlab with Tampermonkey

This Tampermonkey script allows you to easily upload your Claude AI chats to a Gitlab repository directly from the chat page. With just a few clicks, you can save your conversations and store them in a structured manner on Gitlab.

## Features

- Automatically adds an "Upload To Gitlab" button to the Claude AI chat page
- Supports creating new chat files or updating existing ones in the Gitlab repository
- Allows specifying a custom path within the repository to organize chat files
- Retrieves the chat data from the Claude AI API and uploads it to Gitlab
- Opens the Gitlab URL of the uploaded chat file for easy access
- Persists Gitlab configuration (domain, token, project ID, branch, path) for convenience

## Installation

1. Make sure you have the Tampermonkey browser extension installed in your web browser.
2. Open the [raw script file](https://raw.githubusercontent.com/username/repo/main/upload-claude-ai-chats-to-gitlab.user.js) from the GitHub repository.
3. Copy the script source
1. Open Tampermonkey in your browser and click the Add Script tab (icon with a plus symbol)
1. Paste the source into the script window and hit save
1. Voila!

## Configuration

To use this script, you need to configure a few settings:

### Gitlab Personal Access Token

1. Go to your Gitlab user settings by clicking on your profile picture and selecting "Preferences".
2. Navigate to the "Access Tokens" section.
3. Click on the "Create personal access token" button.
4. Give the token a name and select the "api" scope.
5. Click on the "Create personal access token" button to generate the token.
6. Copy the generated token and keep it secure.

### Gitlab Project ID

1. Open your Gitlab repository in a web browser.
2. Go to the repository's "Settings" page.
3. In the "General" section, you will find the "Project ID".
4. Copy the project ID.

## Usage

1. Open a chat conversation on the Claude AI chat page.
2. Click on the "Upload To Gitlab" button that appears near the chat controls.
3. Fill in the required information in the modal:
   - Gitlab Domain: Enter the domain of your Gitlab instance (e.g., `gitlab.com`).
   - Gitlab Token: Paste your Gitlab personal access token.
   - Gitlab Project ID: Enter the project ID of your Gitlab repository.
   - Project Branch: Specify the branch where you want to upload the chat files (e.g., `main`).
   - Path (optional): Provide a custom path within the repository to organize chat files (e.g., `chats/`).
4. Click on the "Upload" button to upload the chat to Gitlab.
5. The script will check if the chat file already exists in the repository and either create a new file or update the existing one.
6. Once the upload is successful, the Gitlab URL of the uploaded chat file will open in a new tab.

## Credits

This script was written by Claude, an AI assistant created by Anthropic. Special thanks to the Claude AI team for providing an excellent conversational AI platform.

If you have any questions, suggestions, or issues, please feel free to open an issue on the GitHub repository.

Happy uploading!
