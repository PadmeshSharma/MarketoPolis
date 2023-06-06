# NISM-Project
![1920-1](https://github.com/PadmeshSharma/NISM-Project/assets/100578426/fe72e9a4-96fc-4034-8fc1-892d50de9714)

The project was built as a part of the “Investor Awareness Hackathon 2023”. An educated investor is an asset to the Nation. In this purview, SEBI has always taken measures to increase securities market awareness amongst the investors. This era of digitization and involvement of artificial intelligence (AI) in each and every sphere, calls for looking at different innovative ways to spread information amongst investors and for identifying new ways of creating investor awareness.
Link to the project: [MarketoPolis](http:/.com/)

## Vision
“Investor Awareness Hackathon 2023” is an open competition for thousands of enthusiasts who seek to disrupt the current method of disseminating investor awareness amongst investors. The objective of this project is to look forward to various innovative mechanisms through which the investors can be made aware and educated to handle their personal finances responsibly and invest with knowledge.

## Theme
The theme of the project is “Informed and Educated Investor”. The developed tool, mechanism or idea should facilitate in infusing the securities market awareness amongst the general public with wider reach in cost effective manner.

## Problem Statement – Incubating rational investment behavior amongst investors using AI/technology.
![image](https://github.com/PadmeshSharma/NISM-Project/assets/100578426/6c074633-09a2-441b-9d87-b3b21388fb98)
* **In general Scenario, we have accountants if one need to invest in any company or stock market who analyses the market situation and accordingly suggest people to invest in respective company but think…… 
If we have a software for the same which with the help of technology and ongoing market situation assist general people who have not much knowledge about investment.**

Now, It’s a thing to ponder about……
How will It Change Scenarios For Our Investors??

## Solution 
|          |            |           
|----------|------------|
|![image](https://github.com/PadmeshSharma/NISM-Project/assets/100578426/fd5ee223-0706-4620-94b0-141be9c41581)|![image](https://github.com/PadmeshSharma/NISM-Project/assets/100578426/a070caba-2253-4d92-9ea8-a081b765f744)|

![image](https://github.com/PadmeshSharma/NISM-Project/assets/100578426/33bc42c9-729c-4799-87bb-57ac369c4ff6)

## Advantages

|          |            |           |
|----------|------------|-----------|
|![image](https://github.com/PadmeshSharma/NISM-Project/assets/100578426/f8221f18-37aa-4e10-96b6-dfc04fe75fd2) | ![image](https://github.com/PadmeshSharma/NISM-Project/assets/100578426/ca32bfa5-af36-4eb4-8519-c12764ae0182) | ![image](https://github.com/PadmeshSharma/NISM-Project/assets/100578426/6997958b-6776-4230-a9d0-817f11fcc9d3)|
|![image](https://github.com/PadmeshSharma/NISM-Project/assets/100578426/605b9f88-a549-4be8-9bbc-5198a83f854b) | ![image](https://github.com/PadmeshSharma/NISM-Project/assets/100578426/b03c486c-72ff-4cfc-919e-4625bd052bf9) |![image](https://github.com/PadmeshSharma/NISM-Project/assets/100578426/5786cc8b-b08c-4007-8b75-592514d50efe) |

## Competitive Analysis
![image](https://github.com/PadmeshSharma/NISM-Project/assets/100578426/7799a54b-6df6-44ac-b89e-d98702262f8c)





# Features Implemented
1. 

# Tech Stack
<p align ="center">
  
</p>

# Implementation
1. ### Group Video Call Feature
   In the app there are two ways one can have a video call: 
     * Instant meeting
     * Inside the groups<br />
     
   When having a call via the instant meeting, options like chat, notes and surveys is not available. This feature is for those who want to connect but dont want to create a        group or store conversations for later. For making this real time communication possible, **webRTC** with **socket.io** was used to make simple peer connections withing a mesh network. Whenever a new peer joins ze makes a simple peer connection with each of the existing peers. For the audio/video controls and the screen share feature we replace the audio/video track with the desired input. The **simple-peer** library was also used. 
3. ### Database Models for group chat, surveys, connections etc
   For the entire application the database service used was firestore database. On sign up each user gets added into the **users** collection and each document inside the collection(i.e each user) has certain fields like ze's email theme choice etc. Further each user also has a **connections** and **connection requests** collecton inside them. This is helpful in sending and accepting requests. Users that are connected are shown on the connections page and we have the option of creating groups with them. When a group is created the all the selected users get added in that group and the group gets added inside the **groups** collection with each group having a unique ID. Every group then has three more collections namely **messages**, **feedback forms**, **feedback results** and **notes**. The messages are rendered by the ascending order of timestamp. Feedback forms and feedback results further have the creator of the form stored inside them. This is done to avoid creator of the form from filling the form and non creators from seeing the results. When a user creates a notes it gets added inside the notes collection and similarly on deleting a note we delete the document from the notes collection. 
<br />
Since all the messages are getting stored in the database conversations that happen inside the video call are also getting stored and will be available post call.

# Snapshots of the project
<h4>Video Call feature</h4>
<img src="/teamsclone/teams/src/Images/videoCall.jpeg" width=600 height=400>
<br />
<h4>Groups and Chat</h4>
<p float="left">
  <img src="/teamsclone/teams/src/Images/createGroup.png" width=400 height=300 />
  <img src="/teamsclone/teams/src/Images/chat.png" width=400 height=300/>
</p>
<br />
<h4>Numerous themes to choose from</h4>
<p float="left">
  <img src="/teamsclone/teams/src/Images/theme1.png" width=280 height=300 />
  <img src="/teamsclone/teams/src/Images/theme2.png" width=280 height=300/>
  <img src="/teamsclone/teams/src/Images/theme3.png" width=280 height=300/>
</p>
<br />
<h4>Survey forms</h4>
<p float="left">
  <img src="/teamsclone/teams/src/Images/feedbackCreate.png" width=280 height=300 />
  <img src="/teamsclone/teams/src/Images/feedbackFill.png" width=280 height=300/>
  <img src="/teamsclone/teams/src/Images/feedbackResult.png" width=280 height=300/>
</p>
<br />
<h4>Notes Section</h4>
<img src="/teamsclone/teams/src/Images/notes.png" width=600 height=400 />
<br />
<h4>Profiles, users and connections</h4>
<p float="left">
  <img src="/teamsclone/teams/src/Images/profile.png" width=280 height=300 />
  <img src="/teamsclone/teams/src/Images/users.png" width=280 height=300/>
  <img src="/teamsclone/teams/src/Images/connectionRequests.png" width=280 height=300/>
</p>

# Major Learnings
1. **Agile Methodology**: Through the 4 week span of the project, I undertook weekly sprints and made sure that small features get implemented in an efficient and time bound manner. Having a usable version of the product from the very beginning and seeing it evolve through the days and weeks was a joyful experience.
2. **Perseverance and debugging skills**: Having faced numerous bugs that seemed *impossible* to solve at first to actually overcoming them felt like victory. It improved my problem solving skills and faith in hardwork.
3. **New Technologies**: The project was a fun introduction to webRTC, sockets and databases for me and I thoroughly enjoyed learning the new technologies. With the help of my friends and mentors as well as self study I was able to grow my knowledge.
4. **Growth mindset**: The sessions as well as the project taught me that our skills can be improved and having a growth mindset helps one and their organization in the long run.
 

## Plans for the future

We are planning to add more and more features to this project. For this, we need your help! Find out how to contribute below. 👇

## Contribution

Any contributions are highly appreciated. :pray: You can contribute in two ways:

1. create an issue and tell us your idea :bulb:. Make sure that you use the **new idea** label in this case;
2. fork the project and submit a PR with your new idea. Before doing that, please make sure that you read and follow the [Contribution Guide](./CONTRIBUTING.md);


## Spread the word!

If the information from this repo was useful to you in any way, make sure you give it a star 🌟, this way others can find it and benefit too! Together we can grow and make our community better! :smiley:

Do you have any suggestions on how we could improve this project overall? Let us know! We'd love to hear your feedback!


