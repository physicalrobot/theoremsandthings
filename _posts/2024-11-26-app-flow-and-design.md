---
layout: post
title:  App Flow and Design
description: Developing with direction and purpose.
date:   2024-11-26 15:01:35 +0300
image:  '/images/UX-flow-chart-min.jpg'
tags:   [Developer, KnowGo]
---

# Progress Update: Figuring Out the App Flow 🚀

Hey everyone! Excited to share some progress on my app, KnowGo! Over the past few days, I've been deep in the process of figuring out how the app will flow and how to structure the user experience. This is a very important part of the development process, and frankly will really make or break the whole thing. 

## The Big Decision
After brainstorming and exploring a few interface ideas, I decided to create <span style="color:turquoise;">**separate profiles**</span> for tutors and students. This approach allows me to design features that cater specifically to the needs of each type of user.

## Designing the Sign-Up Process  
One of my goals is to make the app as intuitive as possible:  
- <span style="color:turquoise;">**Students**</span>: A streamlined and quick sign-up process with just a few simple steps.  
- <span style="color:turquoise;">**Tutors**</span>: A more thorough process involving additional checks and balances to ensure quality and safety before their accounts go live.

Once I had a basic layout in mind, I turned to <span style="color:turquoise;">**Figma**</span> to bring it to life. My fiancé Sara, who’s an amazing <span style="color:turquoise;">**UX Designer**</span>, was a huge help in refining the design and layout. Her expertise made the process much smoother and gave the app a polished look!

<p align="center">
  <img src="{{site.baseurl}}/images/signupflow.png" alt="sign up flow">
</p>

## Building the Backend with Firebase  
On the development side, I’ve been learning and working with <span style="color:turquoise;">**Firebase Firestore**</span> to create a user database specific to their role. <span style="color:turquoise;">Tutors</span> accounts will have more information saved in the database than <span style="color:turquoise;">student</span> users.  

Firestore’s flexibility has been great for organizing these details and laying the groundwork for future features.


## Student User Object
```json
{
  "name": "John Doe",
  "email": "johndoe@example.com",
  "subjects": null,
  "location": null
}
```
## Tutor User Object
```json

{
  "name": "Jane Smith",
  "email": "janesmith@example.com",
  "subjects": ["Math", "Science", "English"],
  "location": {
    "latitude": 37.7749,
    "longitude": -122.4194
  }
}
```

---

I’m thrilled with the progress so far and excited to keep building! Next steps include implementing the sign-up process in the app and connecting it to the database.

As always, I’d love to hear your thoughts or suggestions!
