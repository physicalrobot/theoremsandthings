---
layout: post
title:  Learning Firebase
description: Complicated Logistics Made Simple 
date:   2024-11-18 15:01:35 +0300
image:  '/images/firebase-header.png'
tags:   [Software Engineering, KnowGo]
---

### Why Firebase?

Firebase offers an all-in-one solution for app developers. Its diverse features, including real-time databases, authentication systems, and serverless functionality, make it an ideal choice for startups or solo developers looking to focus more on app logic than backend infrastructure. Below are the Firebase features I’ve implemented so far in KnowGo:

  - Authentication: Simplifies user login and sign-up processes.
  - Cloud Firestore: A powerful, scalable NoSQL database for storing and syncing app data in real-time.
  - Firebase Hosting: A reliable way to deploy and host web applications.

  <p align="center">
  <img src="{{site.baseurl}}/images/firebasemanage.jpg" alt="firebase summary">
</p>

### Learning Firebase Authentication

## What It Does
Authentication is often the first step in app development to establish user identity securely. Firebase Authentication supports various methods, including:

 - Email and password authentication.
 - Third-party providers (e.g., Google, Facebook, GitHub).
 - Anonymous authentication for quick testing.

 <p align="center">
  <img src="{{site.baseurl}}/images/auth.png" alt="authorization">
</p>

### Implementation in KnowGo
For KnowGo, I wanted users to log in with their email and password. Firebase's pre-built authentication methods provided an easy way to set this up without diving into complex backend code. Here’s what I learned:

 1. Setting Up Authentication:
    - Configuring Firebase Authentication in the Firebase Console was straightforward. By enabling the email and password method, Firebase handled password storage and verification securely.

 2. Using the Firebase SDK:
    - The Firebase SDK made it seamless to integrate authentication into my app. For instance:

```
  import { getAuth, signInWithEmailAndPassword } from "firebase/auth";

  const auth = getAuth();
   signInWithEmailAndPassword(auth, email, password)
    .then((userCredential) => {
    // Signed in
    const user = userCredential.user;
    console.log('Logged in user:', user);
   })
    .catch((error) => {
    console.error('Authentication error:', error.message);
   });
```
---

### Firebase Hosting
To showcase the progress on KnowGo, I needed a platform to deploy the frontend. Firebase Hosting came to the rescue. It provides:

 - Fast and secure static site hosting.
 - Built-in integration with Firebase services.
 - Easy deployment using the Firebase CLI.

## Steps Taken
1. Setup:
   - I initialized Firebase Hosting in my project using the CLI:

   ```
   firebase init hosting
   ```
2. Deployment:
   - After configuring the build directory, deployment was a single command:

   ```
   firebase deploy
   ```
3. Result:
    - The site was live within minutes, ready to showcase KnowGo’s frontend to collaborators.

---
### Challenges and Learnings
While Firebase simplifies many aspects of app development, there were a few challenges I encountered:

 1. Understanding Firestore Queries:
   - Firestore's querying capabilities are powerful but have limitations, such as the inability to perform complex joins. I had to rethink my data structure to optimize for Firestore's querying model.
 2. Handling Authentication Errors:
   - Error messages during authentication were sometimes vague. Using Firebase’s extensive documentation helped troubleshoot issues effectively.
 3. Deploying Changes:
   - While Firebase Hosting is efficient, remembering to redeploy after every frontend change required discipline and automation in the workflow.

### Conclusion
Learning Firebase has been an enriching experience. Its comprehensive suite of tools allowed me to rapidly prototype and build critical parts of KnowGo. From setting up user authentication to storing and syncing data in real-time with Cloud Firestore, Firebase provided the foundation for the app’s development.

Personally, I'm sold on this service. Firebase has made so much of the backend work easy and streamlined. As I continue building KnowGo, I’ll explore more Firebase features, such as Cloud Functions and Analytics, to further enhance the app. Stay tuned for more updates as I log my development journey!

<p align="center">
  <img src="{{site.baseurl}}/images/firenationarmy.jpeg" alt="join the fire nation">
</p>

