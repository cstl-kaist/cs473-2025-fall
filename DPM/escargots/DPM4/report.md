
# Project Summary

Gym-goers often struggle with maintaining consistent attendance due to fluctuating self-motivation. Our app uses gamification and peer interaction to address this by introducing features like motivational pokes, shame posting, and an XP-based leaderboard. This approach uniquely combines social accountability and competition, inspiring users to engage more actively with their fitness goals.

---

## Instructions

### Receive a Poke and Test It Yourself

(Since real-time poking by others isn’t available for testing purposes, you can simulate being poked by using the feature to poke yourself.)

1. **Send a Poke**:
    - Select yourself from the poke list.
    - Choose a poke type:
        - **Just Poke**: Gentle nudge.
        - **Join Me**: Invitation to work out together.
        - **Trash Talk**: Playful challenge.
    - Gain 10 XP for motivating someone.
2. **Receive the Poke**:
    - **Check Push Alarm**: Once you’ve poked yourself, you’ll receive a push notification on your device, just like you would when poked by a friend.
    - **View Notifications**: Open the app and tap on the notification bell icon to access the notification board and view the details of the poke you received.

### Shame Post a Friend

1. **Shame Post**:
    - Select a highlighted name from the poke list.
    - Choose "Shame Posting."
    - Use the app's Instagram story template to create and share the post.
    - Gain 50 XP for completing the shame post.
2. **Refresh Leaderboard**:
    - Scroll down to refresh the leaderboard and check the updated standings.

---

## Prototype URL

You can run the server yourself following the Readme file in server git repo. While we are planning to run the remote server as long as possible, the remote server might be disconnected due to billing issue.

In this case, please use following info to setup properly.

`<db_username>= wintertree <db_password>=wintertree` 

[Prototype Dropbox Folder](https://www.dropbox.com/scl/fo/ndeewwtga0v147aee4l4q/AEqqqlbzq9BQEh4H9oEX13I?rlkey=5knyancd7qppfydn6th4fnefv&st=g61mws8b&dl=0)

---

## Git Repo URL

- **Server**: [Server Repository](https://github.com/moom-ugrd-24f/poke-n-pump-server)
- **App**: [App Repository](https://github.com/moom-ugrd-24f/poke-n-pump-app)

---

## Libraries and Frameworks

- **Client Application**
    - Expo
    - React
    - React-Native
- **Server**
    - Node.js
    - MongoDB Atlas
    - AWS EC2 instance

---

## Individual Reflections

### Sejun

I was responsible for developing the server side of the application. My role included creating the app’s server, defining schemas using MongoDB, and implementing API endpoints. Initially, I built and tested the server locally, sharing progress with my teammates through a Git repository. Later, I deployed the server on a remote AWS instance to allow the team to access it seamlessly.

The most challenging aspect was troubleshooting frequent access errors when working with the remote server. While setting up the AWS instance, I encountered various errors that made it difficult to establish a stable connection. At one point, I reduced the security group settings to troubleshoot, which unfortunately led to a brute force attack on the server. To resolve this, I reconfigured the security group to enforce strict IP-specific access, which finally allowed us to work securely and stably. 

Throughout the project, I gained many new skills, such as using Git effectively, setting up AWS instances, and managing MongoDB. However, the most valuable skill I learned was **analyzing server logs for debugging remote server issues**. By reviewing logs, I was able to identify and resolve connection issues efficiently. This experience taught me how to approach server-related problems systematically, making me more confident in managing remote servers in future projects.

### Yeongung Kim

- I developed client application together with Paul Guerre. Specifically, I implemented UIs our team proposed in the lo-fi prototype, handled local user data and called server APIs.
- The most frustrating part was that I had no previous experience of Expo framework, nor React Native or even React. There were lots of new concepts that I had to get used to, which are specifically used in React projects. Also, separation between UI components and data layer architecture were different from previous experiences, which made it harder to manage data. Additionally, since the main feature of our service, poking, requires propagating push alarms to specific client devices, there are many limitations in deploying the application, in addition to the multi-platform (iOS and Android) support.

### Paul Guerre

I collaborated with Yeongung Kim in developing the client side of our application using the Expo framework. My primary responsibilities included integrating server API responses into the UI components, ensuring data fetched from the server was properly displayed and updated in real-time. Additionally, I worked on optimizing the app’s navigation and state management.

One of the most challenging aspects was learning the Expo framework and React Native, as I had no prior experience with these tools. Adapting to Expo's structure, understanding React Native's component-based architecture, and handling asynchronous server data were all difficult. I also faced issues with synchronizing server-side updates with the client-side UI, which often required debugging both API responses and state management logic. After extensive testing and research, I implemented efficient methods to handle these challenges, ensuring seamless server-client communication.

Through this project, I gained a strong foundation in Expo and React Native development, particularly in API integration and state management. The main lesson I learned is how to collectively work with the server to troubleshoot and resolve issues quickly.
