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

**Link to work4:** [Meditation-Timer](https://github.com/kirbycampbell/meditation-timer-hooks)

###################################################################################################

### Day 5 : March 19, 2019

**Today's Progress**:Refactored The Meditation app into containers. Figured out the difference between regular React/Props and ReactHooks/Props - Passing Down UseState into the Components!

**Thoughts:** : Broke through on my props issue, Organized the project so much more! Next up is making each user selection show up and effect it's own state for the background music, the end sound, and the timer. Need to add ability to save Different Timers.

**Link to work4:** [Meditation-Timer](https://github.com/kirbycampbell/meditation-timer-hooks)

###################################################################################################

### Day 6 : March 20, 2019

**Today's Progress**: Began a new project that will become my official/printable resume for job hunting.
I styled purely in CSS, and rendered with jsx in React. Overcame many css grid obstacles, and began planning my personal info that will go inside of the resume.

**Thoughts:** : Initally had trouble laying out the grids correctly, but eventually got it looking amazing.  
Added Dividers in between each section too.  
For right now there are still borders around each section.  
Those will be removed once all of the typed info is in place.  
It's good to see the boundaries and expand and contract as neccessary.

**Link to work4:** [Resume](https://github.com/kirbycampbell/kirby-resume)

###################################################################################################

### Day 7 : March 21, 2019

**Today's Progress**: Began another new project - called Chat_App for now...
I began with experimenting with GraphQL Schemas, and running into brick-walls with aws amplify as its been a month since I've worked in that setting.

**Thoughts:** : The Chat app is aiming to be a fully featured web chat program, with the ability to live chat (seeing each letter as its typed if the users choose so) while also allowing message editing to avoid \*typocorrection messages.
Hopefully this app could be converted into a React Native app for android SMS messaging, or simply existing like a Whatsapp program but with more features.

**Link to work4:** [Chat_App](https://github.com/kirbycampbell/chat_app)

###################################################################################################

### Day 8 : March 22, 2019

**Today's Progress**: Continued working on the Chat app and its backend through AWS/Amplify GraphQL.
Successfully defined a simple schema for the messages only, and implemented functions within my that could mutate, query, and subscribe to the Hosted Backend.  
The App Auto loads the messages now with the newest message at the bottom, with an auto scroll to the bottom.  
Anytime a new message is sent, the chat is automatically updated and scrolled to the bottom as well.

**Thoughts:** : Had some holds ups when I got to the subscription material, but I ended up including it in the open within my React Class.  
Also had a bit of trouble setting up the auto-scroll upon receiving new messages, It works right now, but not consistently... We shall see about that.
Also did some styling and css in general.

**Link to work4:** [Chat_App](https://github.com/kirbycampbell/chat_app)

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

**Link to work4:** [Chat_App](https://github.com/kirbycampbell/chat_app)
