Reddit Saved Posts Downloader
A simple, user-friendly Windows application to download your saved posts from Reddit, including post details and images. You can also choose to automatically unsave posts after downloading them.

Important Limitation
Due to a limitation in the Reddit API, this tool can only access the 1000 most recent saved posts. It cannot retrieve saved posts older than that, even if they are still present in your account.

Features
Graphical User Interface: Easy-to-use interface, no command-line knowledge needed.

Multiple Export Formats: Save posts as text files with separate images, or as a single .docx file with images embedded.

Full Image Support: Downloads single images as well as all images from multi-image gallery posts.

Unsave Functionality: Optionally unsave posts automatically after they have been successfully downloaded.

Connection Testing: A built-in test button to verify your API credentials are correct before you start.

Secure & Private: Your password is only used for the session and is never saved to disk.

Setup Instructions
Step 1: Get API Credentials
You need to tell Reddit you are creating a script to access your account.

Log in to your Reddit account and go to the Reddit Apps page.

Click "are you a developer? create an app..." at the bottom.

Fill out the form:

name: My Downloader (or anything you like)

Select script for the app type.

redirect uri: http://localhost:8080

Click "create app".

You will now see your app's details. You will need two pieces of information:

The string under "personal use script" is your Client ID.

The string next to "secret" is your Client Secret.

Step 2: Install Python
If you don't have Python, get it from the official website. It's crucial that you allow the installer to add Python to your system's PATH.

Go to python.org/downloads/ and download the installer.

Run the installer.

Make sure to check the box that says "Add Python to PATH" during installation. This is very important.

Complete the installation.

Step 3: Install Libraries
Open the Command Prompt (search for cmd in the Start Menu) and run the command below to install all the necessary libraries for the application to function.

pip install customtkinter praw requests Pillow python-docx

How to Run
Save the Python File
Save the reddit_downloader.py file to a new folder on your computer (e.g., on your Desktop).

Navigate to the Folder
Open Command Prompt and navigate to the folder where you saved the file. For example, if you saved it in a folder named "RedditDownloader" on your Desktop, you would use this command:

cd Desktop\RedditDownloader

Run the Script
Run the script using the following command. The application window will open.

py reddit_downloader.py

Fill in Details & Start
Enter your Client ID, Client Secret, username, and password into the application, select your options, and click "Start".
