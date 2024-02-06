# **YouTube Application with RabbitMQ**

# Overview:
This project implements a simplified version of a YouTube application using RabbitMQ, consisting of three components:

2a. YouTuber:
- Allows YouTubers to publish videos on the YouTube server.
- YouTubers can publish videos by sending messages to the YouTube server, including video and YouTuber names.
  
2b. User:
- Users can subscribe or unsubscribe to YouTubers by sending messages to the YouTube server.
- Real-time notifications are received whenever a subscribed YouTuber uploads a new video.
- Users can log in using the User.py script with their name as the first argument. Optionally, they can subscribe or unsubscribe to a YouTuber using the second and third arguments.
- Users receive notifications for videos uploaded by their subscriptions during their absence.

2c. YouTubeServer:
- Consumes messages from Users and YouTubers and stores them as data.
- Maintains lists of YouTubers and their videos, as well as all users and their subscriptions.
- Processes subscription and unsubscription requests from users.
- Sends notifications to all subscribers of a YouTuber whenever a new video is uploaded.
  
# Getting Started
1. Clone the repository.
2. Set up RabbitMQ on your local environment.
3. Run the YouTuber, User, and YouTubeServer components as instructed in their respective sections.

# Usage
YouTuber
- Execute the YouTuber script to publish videos.

User
- Run the User script with your name as the first argument to log in.
- Optionally, subscribe or unsubscribe to a YouTuber using the second and third arguments.

YouTubeServer
- Start the YouTubeServer to handle user subscriptions, video uploads, and notifications.
