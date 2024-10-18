# News App

This project is a simple web application that fetches news articles from two servers (primary and backup) using JavaScript. The application allows the user to click a button to retrieve news articles, display them in a list, and handle any potential errors gracefully. A spinner is displayed while the news is being fetched, and an error message is shown if both servers fail to respond.

## Features

- **News Fetching**: Fetches news articles from two different sources using Promises.
- **Fallback Mechanism**: Uses a backup news server if the primary server fails.
- **Loading Spinner**: Shows a loading spinner while news is being fetched.
- **Error Handling**: Displays an error message if both servers fail to return news.
- **Source Display**: Shows the source from which the news was fetched.

## How It Works

1. **Click the Button**: The user clicks the "Get News" button.
2. **Fetching Data**: The app tries to fetch news from the primary server.
   - If the primary server fails, the app automatically fetches from the backup server.
3. **Loading State**: While fetching, a spinner is displayed to indicate loading.
4. **Success**: The news articles are displayed in a list with their source.
5. **Failure**: If both servers fail, an error message is displayed.
