# 100 Days Of Code - Log

###################################################################################################

### Day 0: March 14, 2019

**Today's Progress**: Added Social Box and CSS to BlogCreator(Medium Knockoff).
Created Twitter account for coding only and began my posting-spree!
Also added automatic loading to the Blog Creator page, so that previous work is auto-reloaded when returning to page.

**Thoughts:** Used some fontawesome icons and placed them on the left side of the page permanently, much like medium.com.
Changed the Desktop View of my blog list to a 2-column view while adjusting spacing.
Ran into a little trouble playing with the grid rows/columns

- it interacted with my footer in odd ways that took some experimentation to figure out.
  Couldn't get the fontawesome icons any bigger,
  I believe that's part of the limitation of fontawesome "free" icons though. Great first day!

**Link to work0:** [Blog-Site](https://github.com/kirbycampbell/blog-site)

# 100 Days Of Code - Log

###################################################################################################

### Day 1 : March 15, 2019

**Today's Progress**: Moved My Firestore app config in blog-store over to a .env file unsuccesfully - attempting to add Auth to my blog-store app.
Seemed like too big of a beast to tackle today, so moved onto a new app that Auth's with firestore, that I can use as an example in the app that already writes to the Firestore db

- without breaking it.  
  Also began work on a simple timer - to serve as a reminder for javascript Date functions.

**Thoughts:** Got stuck working on the Auth - as my BlogCreator has only certain pages requiring login,
and Firestore was a bit complicated in that realm.
So to accomplish something on Day 1 - I built the beginnings of a simple Timer app that I will soon build out as a nicely styled Meditation Timer.
As of now it's crude, but it's doing things!

**Link to work1:** [Blog-Site](https://github.com/kirbycampbell/blog-site)(https://github.com/kirbycampbell/simple-reminder)

###################################################################################################

### Day 2 : March 16, 2019

**Today's Progress**: Made minor stylizing progress with Meditation counter app -

**Thoughts:** time was crunched due to massive 10k+ power outage in portland... 12 hours without power on day 3 of 100 days of code - will do 5x the work tomorrow to make up for the city's disaster.

**Link to work2:** [Blog-Site & Meditation-Timer](https://github.com/kirbycampbell/blog-site)(https://github.com/kirbycampbell/simple-reminder)

###################################################################################################

### Day 3 : March 17, 2019

**Today's Progress**: ReWrote the Meditation Timer from the ground up in React Hooks as a new challenge.
Implemented a custom hook from Dan Abramov called useInterval.
Added Howl library for playing a peaceful gong sound when meditation is over.
Changed form protection - only accepts numbers from 1-140.

**Thoughts:** : Ran into some new issues with setInterval and setTimeout not functioning properly with React's new Hooks update.
Otherwise I love the new Hook's useState syntax, so visually appealing now,
and much easier to implement state changes without the "this" keyword.
Combed through several Audio libraries for react and landed on Howl

- worked great for the gong sound at the end.

**Link to work3:** [Meditation-Timer](https://github.com/kirbycampbell/meditation-timer-hooks)

###################################################################################################

### Day 4 : March 18, 2019

**Today's Progress**:Expanded the Meditation App with Pop up Menu (hand-coded and styled) and added buttons and hamburger. Also Added a Title banner with background image. Mainly styled for mobile thus far.

**Thoughts:** : Hooks has definitely been a learning experience.
Props don't behave like they used to...
It was also pretty hard to find any examples of props being used with Hooks.
Thus far my entire project is within the App.js file since I'm avoiding breaking it down into seperate components and containers.
I need to figure that out soon, as the app is about to get much more complicated!

**Link to work:** [Meditation-Timer](https://github.com/kirbycampbell/meditation-timer-hooks)

###################################################################################################

### Day 5 : March 19, 2019

**Today's Progress**:Refactored The Meditation app into containers. Figured out the difference between regular React/Props and ReactHooks/Props - Passing Down UseState into the Components!

**Thoughts:** : Broke through on my props issue, Organized the project so much more! Next up is making each user selection show up and effect it's own state for the background music, the end sound, and the timer. Need to add ability to save Different Timers.

**Link to work:** [Meditation-Timer](https://github.com/kirbycampbell/meditation-timer-hooks)

###################################################################################################

### Day 6 : March 20, 2019

**Today's Progress**: Began a new project that will become my official/printable resume for job hunting.
I styled purely in CSS, and rendered with jsx in React. Overcame many css grid obstacles, and began planning my personal info that will go inside of the resume.

**Thoughts:** : Initally had trouble laying out the grids correctly, but eventually got it looking amazing.  
Added Dividers in between each section too.  
For right now there are still borders around each section.  
Those will be removed once all of the typed info is in place.  
It's good to see the boundaries and expand and contract as neccessary.

**Link to work:** [Resume](https://github.com/kirbycampbell/kirby-resume)

###################################################################################################

### Day 7 : March 21, 2019

**Today's Progress**: Began another new project - called Chat_App for now...
I began with experimenting with GraphQL Schemas, and running into brick-walls with aws amplify as its been a month since I've worked in that setting.

**Thoughts:** : The Chat app is aiming to be a fully featured web chat program, with the ability to live chat (seeing each letter as its typed if the users choose so) while also allowing message editing to avoid \*typocorrection messages.
Hopefully this app could be converted into a React Native app for android SMS messaging, or simply existing like a Whatsapp program but with more features.

**Link to work:** [Chat_App](https://github.com/kirbycampbell/chat_app)

###################################################################################################

### Day 8 : March 22, 2019

**Today's Progress**: Continued working on the Chat app and its backend through AWS/Amplify GraphQL.
Successfully defined a simple schema for the messages only, and implemented functions within my that could mutate, query, and subscribe to the Hosted Backend.  
The App Auto loads the messages now with the newest message at the bottom, with an auto scroll to the bottom.  
Anytime a new message is sent, the chat is automatically updated and scrolled to the bottom as well.

**Thoughts:** : Had some holds ups when I got to the subscription material, but I ended up including it in the open within my React Class.  
Also had a bit of trouble setting up the auto-scroll upon receiving new messages, It works right now, but not consistently... We shall see about that.
Also did some styling and css in general.

**Link to work:** [Chat_App](https://github.com/kirbycampbell/chat_app)

###################################################################################################

### Day 9 : March 23, 2019

**Today's Progress**: Today I expanded my Auth functionality on the Chat App.
-Also restyled the app to a dark mode while I'm in production (easier on the eyes).
-I created a NavBar, which adds a User Sign in Functionality - though I still need to implement the login feature now that I've figured out how to Authorize without using CognitoUserPools through AWS, which were causing massive issues (like the lack of ability to search for users in the listUsers function provided by AWS...).  
-I also broke out the NavBar component into its own component, and then converted it over to React Hooks syntax (because I love Hooks).  
-Overall - incredibly productive day on the backend side of things!

**Thoughts:** : The app doesn't "look" too much different from yesterday, but the backend and my understanding of AWS amplify has drastically changed.  
I felt overwhelmed for much of the day, and I'm ending feeling like I "Broke through" with a side of confidence.  
Now that I ditched AWS Auth, I plan to just use bcryptjs to hash and unhash the passwords, and have the entire app live within an authenticated Component, of my own making.  
This will then allow specific chat rooms with each user.
It's coming together... GraphQL MongoDB AWS Backend is working great with amplify, front end is querying, mutating, and subscribing correctly to that backend, and I'm no longer having Auth issues... Great code day!

**Link to work:** [Chat_App](https://github.com/kirbycampbell/chat_app)

###################################################################################################

### Day 10 : March 24, 2019

**Today's Progress**: So MUCH Code. Watched hours of video on useEffect and useReducer Hooks - gained much better understanding of them.  
Utilized the new techniques and converted my entire chat app to React Hooks from regular React.  
Began with just converting individual components to Hooks, out of all code initially living in App.js.
Overcame props roadblock, and sent variables from lower component children up to higher level parents.
Moved Queries into the components they belonged with, and converted code as neccessary(spreading prevState was new syntax in Hooks).
Similarly, added the subscriptions into my Hooks components, and used the useEffect hook to call both Queries, Mutations, and Subscriptions from my Graphql DB.
Ended with a massive laying down of comments.
And p.s.'d the day with a little console.log of each message's id - for editing later.

**Thoughts:** : I really enjoyed the pace of the coding today. Concepts were brand new to me at the beginning of the day (useEffect, props with hooks, etc...) and by the end of the day, I was using the concepts confidently from memory.  
The App feels like its past the "overwhelming" point, since the backend is in my control and understand, and so is the frontend.  
Once theres a firm grasp on those aspects, the rest feels like "creative" time-- I'm pumped to get back to coding it tomorrow.

TODO: Persist User Sign In - and move it to the App.js file. The FriendList and ChatBox components will render signIn messages. (TypeBox won't show up when not signed in)
TODO: User search function - by name, or ID. (grep the user's search term using queries that use the grep)
TODO: Make text bubbles editable. New Text should be "red". Add an edited "note" and a "plus" button so you can see the old message. (this won't be actually editing but just taking the createdAt and matching the old one. )

**Link to work:** [Chat_App](https://github.com/kirbycampbell/chat_app)

###################################################################################################

### Day 11 : March 25, 2019

**Today's Progress**: ChatApp now only renders list of Users and Open Conversation when User has signed up for an account.  
The Sign Up Button Now turns on a sign up form, which can be cancelled, returning the sign up button.  
The User that signs up now mutates the Backend DB, and then from the App.js the app queries the backend for that user (just as would happen during a login cycle) and if it finds the user, the full user's backend stats are saved and able to be sent into each component.  
Next I added bcryptjs, practiced hashing passwords, and getting correct returns - currently being testing by two buttons:: make password - and check password.  
Great progress today!

**Thoughts:** : I spent most of my time today figuring out the GraphQL Amplify syntax for filtering for a certain username.  
Honestly, it was auto filtering 10 users each time, and checking those ten for my userName - so it failed 70% of the time, which had me confused...
Until I added a much higher limit to the search - and then the filter worked every time.  
Next up, I need to add the bcrypt hashing and comparing to the passwords when the user signs up and when they login.  
Also need to add plain login support.  
And then I can add individual conversations with each User signed up.  
And add a User search function, which live updates as a user types!  
Should be easy now that I've figured out the backend filtering process!
**Link to work:** [Chat_App](https://github.com/kirbycampbell/chat_app)

###################################################################################################

### Day 12 : March 26, 2019

**Today's Progress**: Today I spent a lot of time working on bcryptjs and its functionality in React Components.  
So far it was unsuccessful in sending the hashed password to the database and comparing it to the user's entered password (for sign in) but I will break through tomorrow!

**Thoughts:** : Bcryptjs has a delay when hashing a password, and React Hooks doesn't utilize setTimeout in the same was as regular Javascript, it requires a hook, like I used in the meditation timer.  
So I never figured out my problem today, but I plan to knock it out first thing in the morning.  
The User would click sign up --- the username/password sends to a function that uses bcrypt to hash the password, where that newly hashed password is saved to the state as hashPass.
The hashs pass is then saved to the DB along with the username... but the DB kept denying the hash pass because the hash wasn't created by the time it mutates the back end, even though I ordered them correctly.  
So Tomorrow, I plan to add a 2 second timer, using useInterval, and delay the database mutation until the password is hashed.  
Or use some sort of async/await situation might help!
**Link to work:** [Chat_App](https://github.com/kirbycampbell/chat_app)

###################################################################################################

### Day 13 : March 27, 2019

**Today's Progress**: Accomplished adding bcryptjs password hashing to my auth routing in ChatApp. First the User signs up, the password gets hashed by bcryptjs, I set a 2 second timer off with useInterval hook, and then send the hashed password to the backend. The timer is there to compensate for the slight delay hashing uses. Then the login info is sent to the outer App.js file and then the user is filtered through the database, and the stored hashed password is compared with the one the user entered. I also saved the User's hashed password and username in their localstorage, which gets deleted whenever the user logs out. That way, the user stays logged in once they log in. useEffect hook grabs the localstorage to check if the user left their login info available for keeping them logged in!

**Thoughts:** : Had a lot of fun implementing this today - it actually went pretty smoothly! The localStorage part caused some issues, but I realized I could just compare the user's database hash with the hash that saved on the localstorage, since those will always be the same. Simple if statement before it uses bCrypt.compare.
**Link to work:** [Chat_App](https://github.com/kirbycampbell/chat_app)

###################################################################################################

### Day 14 : March 28, 2019

**Today's Progress**: Spent most of the day using trial and error to attempt mutations to the graphql backend for the ChatApp with relationship GraphQL database connections. I spent a ton of time reading documentation of GraphQL and Amplify and attempting the fixes.

**Thoughts:** : Not everyday can have visible forward progress, especially when the work is all done in the backend. Today was one of those days, I was able to get conversations created in the backend, but unable to add arrays of users to the previously created conversation. Once this ID connection is made, I should be able to render individual chat bubbles. Perhaps injecting the conversation ID into the User model as an array would be the best way. Then I could use each user's ID to search for a matching conversation. Though that would cause problems if user's have multiple group chats with one another. So perhaps conversations need to be their entity, containing users... and including a conversation array, and each post within that conversation can have a "sender" who wrote that message. That way the user is in each chat as if it's a chat room, but only between private members.
**Link to work:** [Chat_App](https://github.com/kirbycampbell/chat_app)

###################################################################################################

### Day 15 : March 29, 2019

**Today's Progress**: Broke through on the backend of the ChatApp after having some issues with Amplify resolvers. Accomplished adding conversation ID's to a user's conversation array. Found the correct syntax in aws Appsync console under the schema for ChatApp. Spent probably 5 hours working on the backend. Very happy with the breakthrough, even though there isn't much thats chagned on the front end yet.

**Thoughts:** : Today was another one of those days where you don't "see" the progress, but it was invaluable work on my backend, and in general - my understanding of GraphQL and Amplify/AppSync AWS stuff. Very happy with it all. I had to change repos since the resolvers ran into an unfixable error with Amplify also - so made a new react app, and just copied all of my files and deps over.
**Link to work:** [Chatterson](https://github.com/kirbycampbell/chatterson)
