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

###################################################################################################

### Day 16 : March 30, 2019

**Today's Progress**: Readjusted the GraphQL schema to give conversations many posts through a join table, on top of the many to many relationship between users and conversations through the UserConvos join table. After amplify pushing all of those schema changes, I ran several tests towards creating a conversation when the user clicks another user, and adding both users to that new conversation. I was then able to console.log the user's database file to see the join table listed within that user's conversation array. It all worked!

**Thoughts:** : Next up tomorrow will be the act of implementing features based on my new breakthroughs! I will first apply a query for the chatbox to search the join table's conversation for the list of posts within the conversation between the two users. I will then add subscriptions for this spcific conversation's Id - (new concept - specific subscriptions vs. wide open subscriptions which I've done before). This is truly getting into the nitty gritty of backend work - and it definitely feels complicated and abstract! But wow does it feel good to have it all working! Oh and I also need to add some verifications for when a user tries to login but mistypes their info, or when the localStorage tries to retreive the wrong user/password (from a previous database- unlikely issue, but could happen.)
**Link to work:** [Chatterson](https://github.com/kirbycampbell/chatterson)

###################################################################################################

### Day 17 : March 31, 2019

**Today's Progress**: Got the Join Tables to successfully add a conversation to a user's backend array. The Conversation ID sends to the outer App.js and can then be used within the TypeBox Component for mutating the posts. Worked on adding Posts to conversations, with some luck, but it's not returning the way I'd like it to. I'll need to play with the schema some more tomorrow to get it saving posts correctly.

**Thoughts:** : I'm still not 100% sure about the way the User & Conversations join and return. I'd attempted a few alternate schema options, but none were giving arrays like this current join table is. I had a breakthrough when I decided to name the UserConvo models as a mixture of both the selected User's Id and the Logged in User's Id - which made the convo between the two users searchable through queries.getConversations with an easy props.selectedConvo + props.user.id variable combination!
**Link to work:** [Chatterson](https://github.com/kirbycampbell/chatterson)

###################################################################################################

### Day 18 : April 1, 2019

**Today's Progress**: First I tackled the Conversation connections, and then was able to query the conversation for it's posts, and load those into the conversation array, which maps onto the DOM. I then added subscriptions and those seemed to be working. After experimenting with 3 users, I realized the subsription wasn't filtering properly, and the messages are limited to 10. So that's the next thing to fix!

**Thoughts:** : I always seem to end the day on a "stuck" point, but today really had several bright points and _hand waving_ successes! Finally tying the Users to the conversations, and no matter which user clicks on the other, the conversation is found. Also finally seeing the convo render on the screen was amazing, and seeing it change when i chose another user. Just need to fix the limit and subscription issue. Also it would be nice to cache every convo that I've opened and then just subscribe to changes or query after opening and compare to the current cache. That way the app is faster. I could place the open conversations in a tab above the ChatBox, or the FriendBox could be all of the open conversations, and I could just create a User Search Function to begin new conversations.

**Link to work:** [Chatterson](https://github.com/kirbycampbell/chatterson)

###################################################################################################

### Day 19 : April 2, 2019

**Today's Progress**: Officially solved the Querying & Subscription Problems with my GraphQL backend on my ChatApp. Now I can switch between conversations with users, and only the messages with that user group shows up. Also implemented Subscriptions correctly! Began cleaning up the dual side issues, but saving further exploration into that topic until tomorrow!

**Thoughts:** : Today was another big "AHA!" moment when I figured out the filtering process, and using the {eq: convoId} GraphQL syntax. Now I really know what those query "filters" mean in the amplify portion of my code. Pretty amazing stuff really! I then tried to log on as a new user, create a conversation with my Main UserNumOne, and type something. First Error- the post shows up on the other screen, no matter who the other user wrote to. So the subscription pulls every new post, its not filtering. Second Error - When a user creates a convo with another user, the other user doesn't seem to have the conversation within their array, because it was returning an error when I clicked on the combination of users for that convo. So I need to check that the Users both have the convo within their arrays, and if not, do something about it!!

**Link to work:** [Chatterson](https://github.com/kirbycampbell/chatterson)

###################################################################################################

### Day 20 : April 3, 2019

**Today's Progress**: Add functionality to the meditation timer app I had been working on a week ago. I added another div beneath the user buttons, describing what each button does. I then connected each button to functions in the outermost component. Those functions then remove the timer view and clear up space for the new forms. I also found new sounds to add to my S3 bucket and added a few into my app with howl.

**Thoughts:** : Now that I've added multiple sounds into my app (can't select them yet) I'm tons of No-Cors-Access-Control errors. I think the issue stems from my files on S3 themselves, so I need to figure that out to avoid memory leaks. Otherwise everything went smoothly adding the new functions and button calls. Wasn't able to put much more than an hour in today, since I had tons of College work to catch up on, as well as Music Production deadlines this week. Feeling incredibly accomplished though!

**Link to work:** [Meditation-Timer](https://github.com/kirbycampbell/meditation-timer-hooks)

###################################################################################################

### Day 21 : April 4, 2019

**Today's Progress**: Solved the dual conversation issue in ChatApp. It involved pulling two query's from the backend and whichever one returned something first is the conversation that both users will see. Attempted building a custom resolver on AWS for subscribing to new posts, havent exactly figured that one out yet!

**Thoughts:** : Another one of those great sighs of relief after solving the conversation bug, which led me straight into road blocks with the subscription issues. The subscription is pulling up every new post created when i subscribe to new posts, regarldess of my filtering. When I subscribe to the updatedConversation, I'm limited with how the conversation returns only 10 posts. The conversation subscription seems to be more correct though, so perhaps that's the route I should take, and find a way to unlock the limit on the conversation subscription!

**Link to work:** [Chatterson](https://github.com/kirbycampbell/chatterson)

###################################################################################################

### Day 22 : April 5, 2019

**Today's Progress**: Worked on Custom subscription resolvers on the AWS Appsync & Amplify schema.

**Thoughts:** : I was attempting to add convo Id's as the element to subscribe to on any given post. That way the subscription would be tied to the conversation, but only pulling new posts that contained that specific conversation Id. When I tried to subscribe to the conversation itself, i was getting back the deeply nested array of posts, but couldn't find a way to alter the limit of 10 on those posts. I also tried sorting that deeply nested array of posts so that I only received the most recent 10, but that didn't work either. So today was more of a frustrated experimentation type of day with no clear success, though I did learn a bit about resolvers in the process, which is great!

**Link to work:** [Chatterson](https://github.com/kirbycampbell/chatterson)

###################################################################################################

### Day 23 : April 6, 2019

**Today's Progress**: Continued working on subscriptions within ChatApp. Created my own subscription constant, and dove deeper into the resolvers on AWS. Even tried altering the arguments allowed, but ran into strange errors. Reverted back to where I left off yesterday by the end, but gained awesome knowledge and confidence in AWS Appsync resolvers and the in depth schema on their platform.

**Thoughts:** : Not everyday is forward progress, some take you sideways. I did learn alot within the AWS Appsync realm, as well as altering resolvers to return specific amounts of items when queried. Next I need to alter the resolvers to sort in ascending order as well. That way the top result is the newly pushed item. Its ideal that the conversation is the subscribed to item, since it is ultimately what is being updated. The limit on te returned posts within that updated conversation is actually desired, since I could actually limit it to a few posts that way it's only querying the db for the newest item. But in order to do that, I need the resolver to only return the newest item from the DB itself, not from within the application. I need to alter how graphql returns information, not how I call it or receive it within the component.

**Link to work:** [Chatterson](https://github.com/kirbycampbell/chatterson)

###################################################################################################

### Day 24 : April 7, 2019

**Today's Progress**: Experimented with React-Motion, React-Transition-Group and general CSS effects within the meditation app. Not sure which one I like best, but React-Motion seems to be the most in depth which gets me excited!

**Thoughts:** : This was another one of those read - try - see - repeat --- type of days. Pretty fun for sure, and learned alot! Tomorrow will be a big coding day, back to full hours of coding, not just 1 or 2 hours like I did each day this weekend!

**Link to work:** [Meditation-Timer](https://github.com/kirbycampbell/meditation-timer-hooks)

###################################################################################################

### Day 25 : April 8, 2019

**Today's Progress**: Successfully implemented subscriptions to only update the conversation being viewed. The Subscriptions no longer update the wrong conversations... the convo.id must match the convo being viewed for that to happen. Also added conditionals for mapping the conversation to seperate css className's dependant on who wrote the message, like a normal sms app. Added css for that to color the message and place them on opposite sides, so that the user will always see their own messages on the left, and the other user's on the right.

**Thoughts:** : So I'm super happy to have finally gotten this feature implemented. This was quite the journey, and I had many other ways I had aimed to accomplish this, but this one just hit me last night, and even though its not the most secure, it works for now. And that's all i really need for now, since I would like to focus on something other than subscriptions for a few days now. Maybe styling is in my future next. I know continuous downward scroll is something I'll need to figure out, and also some error checking for bad login credentials. I'd also like for every user to get a choice of how their colors are perceived on other user's views, as well as their own. Need to add a special scroll bar, and highlight the user that is selected at that moment. Also a user search function would be great, and then only show the users that someone is friends with. But I should also have an auto added friend named "Kirby". Maybe even one named "God" as a joke, with some funny prebuilt AI responses.

**Link to work:** [Chatterson](https://github.com/kirbycampbell/chatterson)

###################################################################################################

### Day 26 : April 9, 2019

**Today's Progress**: Spent today working on the ChatApp some more. Cleaned up my chatbox.js code, simplified when the subscription gets set up to avoid dual subscriptions. I also added plenty of responsive css to style the app for smaller screens and phones. Added a hamburger lines for small phones to conditionally render the friendlist over the chatbox for picking friends on a small screen. For the mobile view I spread the chatbox out to 100% width, and made the send button be 100% wide too beneath the typeBox.js. Subscriptions are no longer doubling either.

**Thoughts:** :
Today finally saw some fresh visual progress which was really exciting after the past week of backend work. I love backend the most honestly, but it really is rewarding to see all of your backend get rendered beautifully to the front end and "just work"! Tomorrow will likely include furthering of styling, better user login experience and buttons, and possibly even the addition of tabs above the chat box, which will be a new component, rendering a certain set of ongoing conversations. Another great feature would be a count of unread messages next to each person's name or an exclamation point. We shall see! I also want to add editable messages if the user wrote the message, that way people can make corrections!

**Link to work:** [Chatterson](https://github.com/kirbycampbell/chatterson)

###################################################################################################

### Day 27 : April 10, 2019

**Today's Progress**: Today I debugged some intense GraphQL errors that showed up out of nowhere, seemed to deal with auth. Tried to replace the auth with amplify cli, but it wouldn't allow me to update. Ended up just rebuilding another create-react-app and copying all of the files over to the new project file. While I was at it, I hosted the project live on the web. Also added a Friend Tab on top of the ChatBox for mobile user's to see who is being chatted with at any given moment.

**Thoughts:** : Today was alot of debugging and rebuilding, of course it was important stuff. Only got to work on new features for about an hour or so. I had to adjust the clicking of a username to send the entire user object instead of just the id- that way the FriendTab can receive all of the selected User's information, and render the name. Soon I need to add an "Unread" message notification. Tomorrow needs to be the restyling day I've been waiting for, as I got stuck doing some more backend work today. It's always fun to see your work visually change and evolve. Possibly might mix in some tailwindcss or bootstrap!

**Link to work:** [Chatterson-Chatapp](https://github.com/kirbycampbell/chatterson-chatapp)

###################################################################################################

### Day 28 : April 11, 2019

**Today's Progress**: Worked through some error handling today. Made sure every login and sign up error was handled. When a user tries to login with a username or password that doesn't exist, it now goes through the correct conditional processes to notify the user and avoid app failure.

**Thoughts:** : It was great diving into the nested conditionals to avoid app failure, as even just part of my else if statements were causing failure when the dbUserInfo object was returned as undefined. Now the app checks if dbUserInfo returns true, if it doesn't it states the failed message, if it does then it checks for username match, and then username and password match, and local storage username and password info compared with the backend info. The only possible failure that might still exist is if I have a user object saved in localstorage, and then rebuild the backend without that user back there. Hopefully now that process just says "user not found", which I believe it should. I won't find out until I rebuild the backend again, or delete all of my data - which will surely happen at some point!

**Link to work:** [Chatterson-Chatapp](https://github.com/kirbycampbell/chatterson-chatapp)

###################################################################################################

### Day 29 : April 12, 2019

**Today's Progress**: Added lots of little features to the ChatApp. Began with adding conditional rendering of the friendTabs and making the CSS work for those auto-columns. Once that worked out, I switched up the friendTab.js to an array state of previously selected Users (aka open Conversations). It also filters out a user if they are already within the openConvo's array.

**Thoughts:** : This is the first step to switching from the friendlist on the right, to using conversation tabs, and friend's lists. I'd like the friendList.js to only list friends (giving everyone 2 friends when they are created). This will then have a search bar at the top of the friendList and will search for usernames as the user types, and give the ability to add friends to their list. This will involve changing the backend for user's, which will now involve adding the friend, which is like creating the userConvo now. Once that userConvo is created they will be added to the friend list, and both users will use that convo to speak. Now convos can be open and closed, and they wll be in a tab when opened. I next need to add the ability to close a tab, and the ability to switch the chatBox when clicking on the tabs as well. So I've got some more work to do!

**Link to work:** [Chatterson-Chatapp](https://github.com/kirbycampbell/chatterson-chatapp)

###################################################################################################

### Day 30 : April 13, 2019

**Today's Progress**: Learned Vue.js for the first time today. Built a todoList in Vue.js inspired by traveryMedia's youtube video - I then converted it into a youtube video watch list. That involved converting all code over to vid syntax and using youtube-embed-vue npm package. Learned the new syntax and applied it into my own version of the app.

**Thoughts:** : I was totally surprised by how familiar Vue.js felt coming from React. It was really a smooth transition, with many common techniques. The main difference was that each file contains all of its styling, naming, state, and templates. Passing the props up and down between parents and children is a bit more verbose than React, but I could see it being convinient for highly secure programs that need that extra optional limitation. Verbose-ness can be useful - so I see the utility of Vue for sure! I also really like how all of the info for that component is in one file, very organized. I'm sure big components get a bit out of hand though!

**Link to work:** [VueApp](https://github.com/kirbycampbell/vueapp)

###################################################################################################

### Day 31 : April 14, 2019

**Today's Progress**: Pushed further in Vue.js. Added Vue Router to my video VueApp. Long-time todoList item began today as well. The goal was to build a copy of a news journal (Council on Foreign Relations) website, and build it from scratch (without looking at their code or anything). I got incredibly far coding their site, completed the navbar, heading, scrollspy functionality, and added a lot of their content to the page. This was great CSS, and HTML practice while becoming more comfortable in the file structure and layout of Vue.js.

**Thoughts:** : For styling a simple app, I really like Vue.js. With the css right below the Html, its so convinient to build a page out. Of course, I know you can do the same in React, but I tend to be a bit more organized in React and keep the css seperate. So maybe I just like vue because it brings out my laziness.
Next up, I need to finish styling out the desktop version of the news Journal knockoff piece, and then add responsive views for larger screens, tablets, and phones - like the original page.
Also need to add the pop up navbar when scrolling downward, and the moving sidebar which locks in place after a certain point.
This app's aim is to show my frontend styling skills and pull off some complicated interactions and animations.
To view the original site check it out here: https://www.cfr.org/backgrounder/naftas-economic-impact
And Check out my version below:
**Link to work:** [JournalApp](https://github.com/kirbycampbell/journalapp)

###################################################################################################

### Day 32 : April 15, 2019

**Today's Progress**: Worked on my Css layout for my Resume built with html/css on top of React. It had been incredibly unresponsive, so I began converting it to a responsive site. I left the vh and vw alone, and switched to percentage and flex/grid based boxes. Took awhile to get them styled similarly. But they are moving a lot better now.

**Thoughts:** : I want to eventually add lots of transitions and extra info that will pop up if a section is clicked or hovered over. It'd be really nice if the app was hyperlinked as well to blog posts of mine, music videos, photos of mixing projects, code snippets. Just overall super interactive for someone to dive deep into before the show up to my website. Should be a fun one!
**Link to work:** [KirbyResume](https://github.com/kirbycampbell/kirby-resume)

###################################################################################################

### Day 33 : April 16, 2019

**Today's Progress**: Continued working on the phone view of my responsive CSS/html resume. Changed Grid column templates, and spacing. Added Media queries.

**Thoughts:** : Felt like a slug today through todays work. For some reason CSS just feels so clunky. If only there was 1 way to do each task made for new frameworks. Like an easier grid based CSS higher level scripting language. Could be a cool project at some point! Regardless, today was definitely some progress on the resume!
**Link to work:** [KirbyResume](https://github.com/kirbycampbell/kirby-resume)

###################################################################################################

### Day 34 : April 17, 2019

**Today's Progress**: Moved all of my Resume pieces into their own components and added materialUI mediaQueries to the mix. Now, two totally different components render based on the screen size, allowing me to totally redesign the resume for phones, instead of just reorganizing the elements. I also added exported consts of my personal information and skill data. Now Each component can just render the data instead of typing my information in each component's view. Keeps the resume dry! Also added a click outside component function to close the contact information view.

**Thoughts:** : Today was super productive- having a well styled resume couldn't be more important for my upcoming job hunt. It was really fun playing with materialUI mediaQueries too. The main trouble I had was the skills box being broken up into multiple grids for the level of experience dots. Finally I got it with no flex or grids or anything, just floats and width. Now I can continue adding my skills, and then add a few more boxes including my projects and education.
**Link to work:** [KirbyResume](https://github.com/kirbycampbell/kirby-resume)

###################################################################################################

### Day 35 : April 18, 2019

**Today's Progress**: Added react-transition-group's CSStransitions to my resume app. Took a bit of fiddling, but I got the transitions to work when the contact buttons are pressed, when a user clicks outside of that area, and when the user clicks the button again to close them.

**Thoughts:** : This transition element will serve as an example for me to create my own transitions and animations in many of my apps. Eventually I want most of my apps to animate when things appear and dissappear, rather than simply appearing. It's much better when things feel truly interactive and futuristic - and this CSSTransition item really helps ease that. I could possibly make an element of a component change state when I hover over it, and when that state changes, the CSSTransition can cause the element to jiggle in place, thus causing every item I hover over to be responsive. This process is much easier than manually building CSS transitions in the css file itself, since CSSTransitions gives you so many callback functions built right in!
**Link to work:** [KirbyResume](https://github.com/kirbycampbell/kirby-resume)

###################################################################################################

### Day 36 : April 19, 2019

**Today's Progress**: Added objects of my work/skills/project information to SkillsData.js to render dynamically on each version of the resume app. Also fully coded out the rows of Programming concepts and rated them based on my level of understanding. Added clickable interactions with the Sections of my resume, so that it can be a clean and simple view of my page. Broke most information out into their own components and css files. Will likely put those in their own folders as well tomorrow, for that totally clean folder heierarchy.
**Thoughts:** : Who would've thought so much work would go into a resume? I definitely imagined it being simpler, but I guess that's what I get making a fully interactive resume!
**Link to work:** [KirbyResume](https://github.com/kirbycampbell/kirby-resume)

###################################################################################################

### Day 37 : April 20, 2019

**Today's Progress**: Serious progress only today! Essentially finished the phoneView.js layout - added footer - added remainder of tabs - made them clickable and minimizeable. Built out the Desktop view almost fully - and did so much alternate styling for it. Added content to SkillsData.js. Hosted the app on heroku. Added a library of emojis to my data as well. OO Yea~~!

**Thoughts:** : Killed it today! Never hit too many roadblocks beyond changing some of the grid layouts to flexbox in the desktop view. Really feel like the resume is coming along and looks close to complete. To finish I'd like to add transitions to the phoneView when opening and closing the sections. Also, I'd like to add little plus signs to show that the sections can be opened. Also I need to slim down the Projects section and only put the name of the project... and when a user hovers it shows the framework info fade in with opacity. On Phones it can have a little plus sign on it for the exrta info and an open button. The School education section can have a link to my flatiron certificate and my GPA standing in school. Each Skill can have a blog post of mine associated with it. Work experience can have links as well. Perhaps even when highlighted. Also need to make COntact info clickable. My face and name should take you to jkirbycampbell.com as well. Three bars on phoneview should give the option for Blog, Share, Print, Contact, and Github.
**Link to work:** [KirbyResume](https://github.com/kirbycampbell/kirby-resume)
