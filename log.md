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

###################################################################################################

### Day 38 : April 21, 2019

**Today's Progress**: Worked on the News Journal Clone app today. Added scrollspy functionality to the side bar. Built out most of the big footer. Added form to the footer.

**Thoughts:** : This one is nearly done. I'll probably add a few links to the paragraphs like in the original next return to this app. I also need to make this app restyle for phones, since all of my apps need to be responsive if possible!

**Link to work:** [JournalApp](https://github.com/kirbycampbell/journalapp)

###################################################################################################

### Day 39 : April 22, 2019

**Today's Progress**: Began a new migration project with learning React Hook's new useReducer Redux replacement as my main goal! I set up the overall project and created the nested flexboxes. I also added onClick handlers to each square after they styled correctly. I experimented with useReducer hook, and then tried to alter a useState object of the game for a bit.

**Thoughts:** : I believe this game will be a good time to use the useReducer hook since it needs to hold a higher state than the players of the game themselves. This way each move can be logged into a higher state, and both players can play with each other. Tomorrow, I need to finish finding a way to alter the state when a specific square is clicked. Perhaps making the state a simple variable in the reducer function will solve the issues. Easy replacement, just grab the variable, and reassign the one element. Each time its called the other variables are altered. When wanting to reset just call the original constant. Also need to build the ai logic in a similar way to my impeccable ruby ai. With a 4x4 game this should present some new ai opportunities though!

**Link to work:** [HikHakJoe](https://github.com/kirbycampbell/hikhakjoe)

###################################################################################################

### Day 40 : April 23, 2019

**Today's Progress**: Got a ton of the game functions working on the 4x4 TicTacToe game (HikHakJoe). I've gotten the useReducer working with a global Redux like state, but with hooks. Now the game is saved within that outer realm, inputs the box checked into an array, which renders into the boxes themselves. I've got conditionals rendering the icons into each square, and the moves switching depending what turn it is. Also provided a block from adding to a prechecked box. Also the game ends when someone has won the game. Also figuring out all 24 winning combos took some drawing to figure out.

**Thoughts:** : Great productive day coding - really enjoyed getting back to the redux style of things - global state rules for games and the like. Tomorrow I'd like to change the "Winner" functionality to a "full board ends the game" type of deal. Also, I plan to add a points system, where a block is worth some points, and a 3 in a row is worth some points, and a 4 in row is worth even more. Would involve keeping track of some complicated logic, but I bet it'd be awesome! I've also got a few ideas for adding points trading for extra moves - to build a meta-game. Or a game where some turns let you place two, but not touching your own piece. Going to be fun!

**Link to work:** [HikHakJoe](https://github.com/kirbycampbell/hikhakjoe)

###################################################################################################

### Day 41 : April 24, 2019

**Today's Progress**: Added the points system to HikHakJoe - and added a meta-game points system. Also made the game continue through multiple "connect-3"'s adding up each connection into the points. Also once the game is over it renders an option to play a new game or end the game.

**Thoughts:** : Another great day working on this app. Super close to getting to the ai portion of coding this app. Next step will include a start screen with the option to play 0-player, 1-player, or 2-player (current mode). To complete some basic functionality I need to add a banner saying who won the game, and change the new game button to (continue). When pressing End Game - i'd also like it to display the final score of both players, giving the option to start over and bring us back to the start screen. In the 1-player game I can begin coding the ai strategies... if 1 space in a win combo is that player, then go for it. I could also return priorities of options, say if 3 options return for building towards a win, the computer can always go for the route with the most available connections. As in - it seems like initially aiming for the middle 4 squares is the smartest, since it opens you up to like 8 possible winning combos. After that - heading for the corners seems smartest. ALSO - adding a checks for win combos that border another matching piece for extra points would be sweet!

**Link to work:** [HikHakJoe](https://github.com/kirbycampbell/hikhakjoe)

###################################################################################################

### Day 42 : April 25, 2019

**Today's Progress**: Did even more work on the HikHakJoe app. Today I added styling to the Points areas below and above, and added messages when games were over. Also added a home screen for selecting 0,1, or 2 player games. Also moved plenty of state from the components into the global state. Began looking for how to restructure app for the incoming ai - as in player moves and calling the ai to return something, and triggering the user again.

**Thoughts:** : So I got sort of stuck on the ai implementation by the end of the day. Though the code is beginning to feel long and jumbled in some spots, so I may need to seperate concerns, because I don't want to exactly call the ai from the boxgrid.js file. The turns and player should probably move back mainly into the global state. Possibly the player can be totally determined in the reducer, in two player games - it could only transmit the block clicked, and then it could just add one to the turn when adding the move to the array. Thats exactly what I should do. TODO ^^^^^. That way the global state can check if the gameType is single, and if so- call a function which will make a move, changing the player's turn back to the users. That should work, but I could forsee a conflict between the function call getting stuck in a dual state with the makeMove call from the ai file. Well, I'll try that out tomorrow for sure! Good starting place.

**Link to work:** [HikHakJoe](https://github.com/kirbycampbell/hikhakjoe)

###################################################################################################

### Day 43 : April 26, 2019

**Today's Progress**: Emplimented many different versions of redux in hikhakjoe, ended up reverting back to normal after some time.

**Thoughts:** : Not much time to write today, will update with what I learned!

**Link to work:** [HikHakJoe](https://github.com/kirbycampbell/hikhakjoe)

###################################################################################################

### Day 44 : April 27, 2019

**Today's Progress**: Coded within the hikhakjoe app while in the woods. Didn't have service to upload my work, but still messed around with reducers and methods for the ai. Also tested my css and expanded on style options I frequently avoid.

**Thoughts:** : About an hour of coding was used to set up my laptop with the correct dependencies for the hikhakjoe app. After that, I had no internet and just had to work however I could on the app. Luckily I experimented a good bit, not making much more forward progress, but trying several ideas out and checking them off the list. Overall great day!

**Link to work:** [HikHakJoe](https://github.com/kirbycampbell/hikhakjoe)

###################################################################################################

### Day 45 : April 28, 2019

**Today's Progress**: Coded some more in hikhakjoe, still experimenting. I think I've got the plan now (on paper) for how to seperate the dual player game from the single player game, which will finally free me up to build the ai out (the supposedly hardest part of this entire thing!). Also began a store-front project.

**Thoughts:** : Excited to start the store-front project since it is pretty much the last type of site I wanted to put on my resume. It should be pretty simple and essentially only show a simple storefront of 8-10 items, and have a cart. I won't add payment or anything like that, just more of a style based app.
**Link to work:** [HikHakJoe](https://github.com/kirbycampbell/hikhakjoe)

###################################################################################################

### Day 46 : April 29, 2019

**Today's Progress**: Redux experimentation and React Custom Hooks documentation deep dive. Switched the checkforWin function over to the global state, I'm questioning my move over though. Sought deeper understanding for what I was aiming to do.

**Thoughts:** : Sometimes forward progress is realizing that you are working sideways, and just searching the documentation for answers is a more productive way. Today was alot of reading, and thinking through my useReducer issues. Is redux really neccessary here? I'm not sure. But I'd like for more than one of my projects to utilize it, so this has to be it, and it could only help the ai stay separated right? We'll see. I'm thinking creating customHooks will be the route to use the checkForWin, gameOver, and points type functions. hopefully that'll extract the logic out of the boxGrid.js, instead of placing it in the reducer like I'm doing now - as I realize this is an anti-pattern. It is currently working though, which is a "win" from the past few days, though I now doubt that its a good convention, and see the issues associated with this style of design. Regardless, this is a serious learing process these past few days, sometimes getting it all "right" isn't much of a learning process, and more of a solidifying your previous knowledge. Today I'd say was adding to my understanding, not neccessarily moving a project forward. But I'm truly understanding why redux should be used a certain way, instead of just following the directions, which is awesome!
**Link to work:** [HikHakJoe](https://github.com/kirbycampbell/hikhakjoe)

###################################################################################################

### Day 47 : April 30, 2019

**Today's Progress**: Finished setting up the redux for HikHakJoe. Dove into the ai full stop. Coded about 400 lines of code for the ai! Built functions for comparing objects, adding up similar items into new objects, sorting for most frequently found item, and all of the decisions that the ai needs to make. I also added the ability for the computer to play itself, and added randomization so that if moves held the same "weight" it would change its move every game it plays.

**Thoughts:** : The ai was super fun to code today, I love working with straight up functions. I think my c++ training is becoming very useful in these situations. This was some serious work today, probably put about 11 hours into the code today. Very focused. I was super pumped to be unstuck from the useReducer/Redux land that was giving me so many issues. Awesome!
**Link to work:** [HikHakJoe](https://github.com/kirbycampbell/hikhakjoe)

###################################################################################################

### Day 48 : May 1, 2019

**Today's Progress**: Practiced a load of C++ classes, variables and structs. More directly for my work I built out the basic frame for my home-website landing page. Began with simple containers, flexboxes, and containers within containers. Then I converted the whole app from the beginning to be responsive. Now I can easily keep both views up to date.

**Thoughts:** : This was a great start, and perfect project for today. Only took me about 2 hours to build out the start to this landing page, which will ultimately be the first thing employers see. From this page they will be able to either click on the resume button, which will provide a pdf button or "live resume app" button. When clicking on the portfolio button it will show my top 4 portfolio pieces with a "click for more" button, which will then load 4 more portfolio pieces. I should also consider adding a "Blog" button to the main screen. Perhaps I should put all of my social media links beneath the Title bar. Github, Twitter, LinkedIn, Email, etc... Regardless of those thoughts, I'd also like to implement some super impressive transitions and interactivity, and maybe even some sliding movements!
**Link to work:** [HomePage](https://github.com/kirbycampbell/homepage)

###################################################################################################

### Day 49 : May 2, 2019

**Today's Progress**: 6 Hours of code spent on C++ project for CompSci 2 class, this shouldn't count, but I did go above and beyond and build extra functions just for added practice. Program works flawlessly. I coded some css for an hour on HikHakJoe 4x4 game - added style to the player's turn notification, fixed some responsive styling, and played with the game select buttons. Also drew out plans for increasing the difficulty of the ai, as it is now easy to beat with my new strategy.

**Thoughts:** : I may keep the current strategy for the ai as "Easy" setting - although it is hard for people who don't know the strategy. And then if someone clicks on the "Hard" strategy, the ai starts calling its harder principles. Essentially those harder principles will start with grabbing all of the center blocks possible, and then trying to "wall" off the opponent. That seemed to work the best for me. Then you just go for wins, and don't even worry about blocking. It's not as intelligent that way though. One thing I would like to add is a points bonus for getting 4 in a row, since that should be "hard" to pull off. So that would entail building some win combos for the four in a rows, and adding that to the iterations for it to aim for. Blocking or going for one of those should be the highest priority. Also adding notifications when a user scores would be sweet, maybe even highlighting the blocks that just made the score! AND, ending the game after the last move, while not requiring that final click would be nice! TOMORROW ITS ON!
**Link to work:** [HikHakJoe](https://github.com/kirbycampbell/hikhakjoe)

###################################################################################################

### Day 50 : May 3, 2019

**Today's Progress**: Did a bunch of debugging work on HikHakJoe and styling. Added Animate.css to the game points section, so when a user scores it bounces the score and says Player 1 Scored! Also added a more responsive layout for the phones, since things were overlapping. I also made the scroll set to center, so that on devices the game is lined up in the middle of the screen. The debugging was involving the way the game handled the end of each game. Previously you had to click the board after the game was over to get the "player 1 wins" message. Now it checks for the game being over with a slew of useEffects and useIntervals to check at the right time.

**Thoughts:** : Fixing that end of game issue was a little tricky, because the ai type games checked for game over in one way, and the user games checked another way. So I needed to convert it to work abstractly. I got stuck on that for probably 2 hours, but pulled through. The code is a little messy, but I'm not sure where to begin on cleaning it up. Maybe putting functions in seperate files for each "type" of function. Like if its ai related, or if its user interaction related. Animate.css was really fun to use as well, I had attempted to use CSSTransition from the react-transition-group npm library, but that proved to be too difficult with my use case. It seems easy to use with clickable boxes and firing off functions when that happens, but the animation I was aiming for would be fired from the global state change, so it was a bit more complicated to tie it in. Plus I wanted both fade in and out respectively, trade places, but only animate.css helped me pull that off. I'd love to get more into interactive animations, I know there are alot more out there than I'm utilizing currently. GREAT DAY 50!!!! HALFWAY!
**Link to work:** [HikHakJoe](https://github.com/kirbycampbell/hikhakjoe)

###################################################################################################

### Day 51 : May 4, 2019

**Today's Progress**: Worked on my resume app. Made the Projects area consistently sized on the phone version. Also added onMouseEnter functions and onMouseLeave functions. These functions send the name of the project to the function, which sets the state to the projects name, and turns on a fade boolean. The classnames get altered depending on if the style is matching the name of that element. This fades out the title, and fades in an absolute element of details. I got stuck when trying to add a background fade in, which requires adding another condtional render to the overall box. but then I powered through that issue for another hour and solved it!

**Thoughts:** : It's always great to finish the night with completing the task you were working on all night. This hover/change styling is much more difficult than I'd antipicated, but I'm building it for robust conditional component rendering so that I can render "Go to site" buttons, and the additional info. So it's super handy. Tomorrow I should probably strip this out into it's own component and just pass in props for each different component. That way I only have to change the code once, not very DRY right now. Going to focus on this tomorrow more for sure!
**Link to work:** [KirbyResume](https://github.com/kirbycampbell/kirby-resume)

###################################################################################################

### Day 52 : May 5, 2019

**Today's Progress**: Debugged some resume & debugged the hikHakJoe app. Kept it simple today!

**Thoughts:** : Excited for this week - lots happening - and lots of projects likely getting much closer to completion! Goal is to have the resume/Portfolio completely done by day 100!
**Link to work:** [KirbyResume](https://github.com/kirbycampbell/kirby-resume)

###################################################################################################

### Day 53 : May 6, 2019

**Today's Progress**: Styled the phone and Desktop View of the resumeApp. Added project styling to desktop. Fixed the dividers in phone view. Added clickable links to the desktop contact area. Positioned items better.

**Thoughts:** : This was some good final style tweaking on this project. Getting close to "send-out" ready! Just need to get the jkirbycampbell.com landing page up and hosted, which can then link to this resume, projects, and my blog. This app also links over to my projects as well. So it's about time that I start organizing all of those hostings and connections. That way I only need to re-push the projects up as they become more polished.
**Link to work:** [KirbyResume](https://github.com/kirbycampbell/kirby-resume)

###################################################################################################

### Day 54 : May 7, 2019

**Today's Progress**: Perfected the Look and Layout of my DesktopView within the resume app. Got the website, and phone links working as well. Fixed all of the border boxes in each section, and made a consistent hover animation for each section. Resized the entire height, which took converting it over to flexbox from grid based. Also tweaked some PhoneView sections as well.

**Thoughts:** : I want to add a print button to the web version of this app, so that people can print or save the pdf image of this resume. I still need to make the Projects section link over to each project (even though not all of the projects are hosted currently). Also I'd like to add some cool little images to the experience cards. Stock Trading - Growth Chart\*. Crypto Rig - Photo of clean rig. Music Producer- Screen shot from Pro Tools.  
**Link to work:** [KirbyResume](https://github.com/kirbycampbell/kirby-resume)

###################################################################################################

### Day 55 : May 8, 2019

**Today's Progress**: Added content to my homepage landing page. Resized overall layout to fit phones and desktops in one screen with no scrollbar. Made transitions to roll the boxes in. Began transitions for the intro welcome message, which triggers the next section.

**Thoughts:** : I need to convert to CSSTransition component to accurately transition between the different states of this app. simple animate.css are too 1 deminsional for the activities I need to build into this app. This app will essentially be my main User Experience app, transitions and interactivity galore. Style needs to be fresh, modern, sleek, and inspiring.
**Link to work:** [Homepage](https://github.com/kirbycampbell/homepage)

###################################################################################################

### Day 56 : May 9, 2019

**Today's Progress**: Made tons of progress on the homepage app. First I added a transitional cssTransition component to the title bar section - added new className assignments in the css file for each transitional name, built specific timing for each transition. Added background images to each Topic Card, Resume-Portfolio-Blog-Bio. Added a background to the 2nd title after the transition. Added bunch of new font options to css file.

**Thoughts:** : For smoothness of this app, I could technically copy all of my other project's code and dependencies into this project, and actually host all of my apps within this one homePage app folder - that way it could quickly load, and just have React Router split up the url's of the pages. Not sold on the top font, but I have a bunch of other fonts saved in the css file. The cards could use some work as well, Font could be better, and the look could be better too... not sure I like the photos in the background. I'd also like to add a social media bar between the title and the main section. Just purely links to social media accounts.
**Link to work:** [Homepage](https://github.com/kirbycampbell/homepage)

###################################################################################################

### Day 57 : May 10, 2019

**Today's Progress**: A bunch more progress on the homepage/landing page. Added cleaner transitions. Added the social bar, redirecting to each different site. Added Bar of buttons once one button is clicked. Also added styles to the selected button, bordering the bottom - to show which is selected. Provided a way out of the bar button view, by clicking an X to get out. Troubleshot some issues on safari with my transitions, have not fixed that issue yet.

**Thoughts:** : Super fun progress! I got stuck when adding CSSTransitions to the boxes transitioning to the bar of buttons... so I left it at an intermediate state. I realized you can't transition between display modes like flex and block, and you cant change the flex mode and have a smooth transition. So that sort of just made me play with opacity transitions, and the buttons fading in. Also I had to add some extra space beneath the buttons or else the footer was climbing up. Tomorrow- I'd like to add the localstorage item that will just present a welcome back message upon re-returning to the site. Also It'd be great to start adding content to the Bio, Blog, Resume, and Portfolio. Shouldn't be too hard. Just straight up hard-coded cards. I should also switch the main four boxes to only have margin-tops since the space in the middle of them is pretty big, seems amateur to leave it like that. I also need to perfect that transition between cards and button row, like i mentioned earlier. See if I can copy code from my blog-site to render all of the blog cards. Could start by just routing to the app itself. Resume will route to 1 card that says Interactive WebApp Resume, or Printable Pdf version. Bio will be new material. This will be the big about me page. I should put a small youtube vide on that page saying hello, and showing my face.
**Link to work:** [Homepage](https://github.com/kirbycampbell/homepage)

###################################################################################################

### Day 58 : May 11, 2019

**Today's Progress**: Transferred some components from blog-site to the homepage. WOrked on styling and db connections to get it all rendering within this app correctly. FlexBoxes don't work well with grids, so layout had to be adjusted to work for this old css I wrote.

**Thoughts:** : This was actually smoother than I imagined, dropping a pre-hooks component in an app written with hooks. The main issues came down to the css flexboxes and grids not playing nicely together. Mainly, the fact that the app was built using view heights, and view widths, really didn't play well with the old grid css stuff. Maybe I'm just realizing that flexboxes are more... flexable - beyond their immediate stretchy meaning. This was some good practice that I probably would have avoided if it hadn't been for this meshing of apps. I should probably build a page using all different types of height elements just to see which ones can do what. That way I can know for certain which types of css displays effect the following items, and which dont. Experimentation time!
**Link to work:** [Homepage](https://github.com/kirbycampbell/homepage)

###################################################################################################

### Day 59 : May 12, 2019

**Today's Progress**: C++ work. Also added a temp backend to the store-front Vintage Store App. I conditionally mapped the temp backend to the frontend and began styling the components. Got the boxes flexing within containers, and holding very consistent. Added images as well.
**Thoughts:** : This was relatively smooth and fun! I'll add a true backend to this one soon, likely a rails backend api just to practice with rails again, its been awhile, and I should keep on my toes with that one! ALso, need to finish styling out the cards with the prices and images. WOuld be cool to have a fun price font and color and place it in a little bubble ontop of the iamges. The title and description can stay below. Also need to add to the navbar, and build out a footer. I should also build out some product pages, for the individual product itself. Show related items (with the same type), and have an add to cart button. Save a user's cart in their local storage. Stop at guest payment processing.
**Link to work:** [Vintage Store-Front App](https://github.com/kirbycampbell/store-front)

###################################################################################################

### Day 60 : May 13, 2019

**Today's Progress**: Added tons to the Vantage Vintage - Vintage store front app. Added some complex footer stylings and added an email form. Played with fonts and added social share buttons to the footer. Built out the navbar as well. Moved all components into their own files and css for better organization. Also built out a filter section which filters through the types of clothing options.
**Thoughts:** : This was really smooth today. I feel like the entire React/Css/Jsx workflow is becoming second nature. I can break things out into new components in seconds, pass props around at ease. It's really starting to feel like I'm getting beyond the "Junior" level of coding, and glimpsing into the senior level, even though my experience is only on my own apps. Just my confidence level from my first few projects after flatiron until now is about 10 fold. Yay to today, I'll take it!
**Link to work:** [Vintage Store-Front App](https://github.com/kirbycampbell/store-front)

###################################################################################################

### Day 61 : May 14, 2019

**Today's Progress**: Added responsive layout to store front vintage app. COnverted css for it.
**Thoughts:** : Small coding day since I needed to catch up on sleep. But regardless I got over an hour in towards this portfolio app.
**Link to work:** [Vintage Store-Front App](https://github.com/kirbycampbell/store-front)

###################################################################################################

### Day 62 : May 15, 2019

**Today's Progress**: Perfected the store front layout within both Desktop view and Phone View. I added Heart buttons to each card on both views, which required layout changes for the cards to use absolute positions. Surprisingly a lot of work reworking the layout setups.
**Thoughts:** : Today was more tedious before I dive into new features, but the layout needed to be solid before I add new features. It's always slower when you try and add new features while trying to fix layout issues as they pop up. Pumped to add some cart adding features, and product page, and checkout page.
**Link to work:** [Vintage Store-Front App](https://github.com/kirbycampbell/store-front)

###################################################################################################

### Day 63 : May 16, 2019

**Today's Progress**: Set up the newly arrived Macbook air, 2014, super affordable coding edition. I fixed container issues for my main homepage cards on safari, while keeping them intact on chrome. Began removing Animate.css, as transitions seem smooth on safari otherwise. New issues arose when I removed Animate.css.
**Thoughts:** : I'm not sure why the ANimate.css classNames are effecting the container bounds for my background images. When I removed the animate classNames, all of the background images grew way outside of their bounds, and aren't responding like they usually do. There must be something else causing it, or perhaps the animate classNames auto set the box sizes for some reason. Regardless, I've gotta figure out, or else I'm going to get rid of Animate.css, since it's introducing these extra variables between browsers. Smoothness is key here, this is my front page. Regardless, I really tried alot of things to fix the containers... these kinds of things always get worked out in my dreams somehow, its wild how helpful sleep can be with problems like these!
**Link to work:** [Homepage](https://github.com/kirbycampbell/homepage)

###################################################################################################

### Day 64 : May 17, 2019

**Today's Progress**: Completely revamped the transitions and css className styling for the homepage app. I also built an example app that I can come back to to see exactly how to build a transitional hooks conditional className app. First I focused on animating the title/Navbar, through its 3 stages using 2 timers. Then I added the social bar, which was the simplest. Then I added the new styling to the Main boxes, and the boxBar (once box is selected) - this took awhile, and still has a little bit of issues. PhoneView is totally off, it needs to be updated to the new process.
**Thoughts:** : This was incredibly productive, as I spent about 10 hours working on this stuff today. I won't type too much, since the smoothness, and clean new code speaks for itself. Hopefully now I can add a couple more transitions, and fill out the rest of the content needed for this project to be done. So close!
**Link to work:** [Homepage](https://github.com/kirbycampbell/homepage)

###################################################################################################

### Day 65 : May 18, 2019

**Today's Progress**: Fixed filtering bugs in store-front Vintage Store app. Fixed styling in that section. Practiced some inheritance and virtual pointers in a local c++ project after reading some c++ textbook stuff. Just over an hour of coding today, needed a little Saturday "downtime" action - but holding strong to my commitment for an hour a day for 100 days!
**Thoughts:** : Pretty great little day! Feeling like I'm really solidifying my c++ knowledge, which in turns helps me apply javascript so much better. Essentially, the more languages I've learned, the more I've "GOTTEN" and understood whats possible in each language, and how to get into my own code flow. Last night I looked back at old projects from the past year, and realized how much more confident, quick, and knowledgeable I am when coding. It really has been such a huge learning process - so valuable, and the amount of time I've put in has seriously been worth it, as this is a solid skill of mine now.  
**Link to work:** [Vintage Store-Front App](https://github.com/kirbycampbell/store-front)

###################################################################################################

### Day 66 : May 19, 2019

**Today's Progress**: Returned to HikHakJoe 4x4 tictactoe game. Built a difficulty selection container, functionality, and global state. This difficulty calls a new harder ai. I recoded ai for the harder version to aim for the center pieces first, and be more aggressive in making it's own winning moves. Also added a footer, which needed me to base all of the styles on percents and veiw heights consistently. Also added like functionality to the store-front app, which also filters for liked items when you click the heart button.
**Thoughts:** : This was some much needed tweaking to this app. It looks pretty good now on safari and chrome, as well as on phones, with some slight footer issues still needing fixing. The harder ai was a simple addition as well, as I only needed to alter a couple modes of its thinking - as in aiming for center pieces first, and then being more aggressive with its moves so it doesnt get caught in defensive land. Next addition needs to be making the games alternate who goes first, and perhaps in the 1 player games calling the ai "Computer" and the human "You" would be helpful. And in the 2 player game, allowing the user's to enter their names would be nice - maybe place a little plus symbol next to the player's turn. Oh I also implemented arrays of moves, so that the order of moves in a game can be kept track of, while also injecting each game into an array of all games & the order in which they were played. That way I could add a sidebar of games played, and when you click on one it can show the order of moves made by which player. Would be pretty interesting!
**Link to work:** [HikHakJoe](https://github.com/kirbycampbell/hikhakjoe)

###################################################################################################

### Day 67 : May 20, 2019

**Today's Progress**: Expanding the homepage app with some components for each main option for the boxes. Built out a portfolio data page instead of using the one from resume. Successfully built out class constructors just like c++ and ruby for creating the portfolio data. That way it can be array mapped and easily rendered out on that section. Began styling some of those components.
**Thoughts:** : Was a little slower with my coding today, even though I spent about 4 hours on it. But that was coming after spending about 5 hours coding my c++ project, but I didn't count that towards 100DaysOfCode since it was for class. So overall, tons of code today, but I was a bit wiped out on it by the end. I find it pretty awesome that the c++ stuff is inspiring me to expand my javascript knowledge, by attempting to pull off similar concepts from other languages. I think this might be the key to truly understanding coding. Applying other languages to each other, and realizing each language's powers and cons. This is what its about.
**Link to work:** [Homepage](https://github.com/kirbycampbell/homepage)

###################################################################################################

### Day 68 : May 21, 2019

**Today's Progress**: Worked on homepage portfolio section's card styles. Added github links to the skills data section. Rendered buttons onto each portfolio card which open a new tab for the code at github or a live demo of the app.
**Thoughts:** : Was productive, but not very quick. I was a bit tired from not sleeping, but got a few hours of coding done. Progress towards the goal!
**Link to work:** [Homepage](https://github.com/kirbycampbell/homepage)

###################################################################################################

### Day 69 : May 22, 2019

**Today's Progress**: Added images to portfolio cards and data. Restructured app so that taller sections push the footer down (was a big issue). Refined styling on the cards in portfolio. Added Resume section content, created space background, padded it and placed the resume pdf inside. Added buttons for printing or the interactive version. Added a loading animation when big cards are clicked and the fade in for the section is happening.
**Thoughts:** : Alright - this is getting close! How about trying to put the actual interactive resume smack dab in the middle of the resume section? Almost should just git it all in one div, and bring it over from that project, should fit flawlessly, once I convert the vh's to 100%'s, keeping it locked into its container instead of using overall vh's. Then I'd only need a print button, download button, or share button.
**Link to work:** [Homepage](https://github.com/kirbycampbell/homepage)

###################################################################################################

### Day 70 : May 23, 2019

**Today's Progress**: Completely rebuilt the Homepage app with a responsive mobile layout, while keeping the Desktop view essentially as I left it, besides a few adjustments. Added new projects to the project section. Also fixed the API issue with the Instant Messenger Chat App, back in business!
**Thoughts:** : I've been on fire lately. Progress has been incredibly noticeable, which normally happens when you live in CSS styling for a week or so. Time to get back to sprucing up the chatApp for the portfolio, and figuring out why my jkirbycampbell.com domain name isn't linking to amplify apps on aws. Once I figure that out, I'll tie the homepage account to it, and have my main page officially live. Then I need to somehow get the Blog Posts rendering, maybe I can pull out parts of the Blog app and slide them directly into my homepage app section. Perhaps making a fork, and changing some stuff within the original app will be the best way to contain the app before moving it over. Make sure css names differ enough too, when they overlap they really mess other things up.
**Link to work:** [Homepage](https://github.com/kirbycampbell/homepage)

###################################################################################################

### Day 71 : May 24, 2019

**Today's Progress**: Eexperimented in C++ with Linked lists. Deployed 2 of my main portfolio apps to add to my portfolio page of homepage app & my resume. Added them to the data in homepage. Practiced some "forgotten" css tricks with see-through borders.
**Thoughts:** : Deployed both of these apps to AWS since they don't have the free teir sleep issues that heroku mandates. I'll likely move all of my projects over to AWS, since My apps can be full speed for the hiring process. Experimented with linked lists in c++ for some deeper practice. Going to hit it all very hard tomorrow!
**Link to work:** [Homepage](https://github.com/kirbycampbell/homepage)

###################################################################################################

### Day 72 : May 25, 2019

**Today's Progress**: Experimented again today - but today with Github's electron, and JUCE c++ audio platform. Set up my first electron app, converted it to a react app template, and then added my Hik Hack Joe 4x4 game app to the template, successfully running my game app as a pure windows desktop app. So cool!
**Thoughts:** : Today wasn't too much forward progress on my legit projects - BUT learning new frameworks and app conversions is soooo useful. The fact that I opened my game as a desktop app, was literally insurmountable yesterday, until I looked into it and learned some electron framework info. Can't believe how manuy apps are built with electron as well, I will definitely be using it some more! Obviously, not many of my apps would be useful as a pure application, but games and the meditation app would be pretty useful! I wonder how my electron apps work when it connects to internet and backend. Also, the Chat App could work really well with electron as well!
**Link to work:** [HikHakJoe](https://github.com/kirbycampbell/hikhakjoe)

###################################################################################################

### Day 73 : May 26, 2019

**Today's Progress**: Worked extensively on the chat app styling and features. Overhauled the styling from grid based css, and converted it to flex boxes which required total switchover. Also adjusted the repsonsive layout. I added a send button to the text area, instead of having a separate button section. The button also conditionally renders based on if there is text in the user text area. Attempted to fix subscription issues to no avail yet.
**Thoughts:** : I remember this subscription issue giving me a real headache a month ago when I was working on this project non stop. After spending about 4 hours on the css and the layout of the app, I tried to figure out the subscription issue, and really just spent most of my time trying to figure out the ways I was calling the subscriptions. I definitely have an issue with the subscription getting called for every new message, even ones outside of the given convo (i filter these out). After that, I need to make sure that the subscription message isn't getting called from within my app multiple times, essentially I need to widdle down if the problem is coming from the aws server, or if my code is dupli-calling the subscriptions method. Also, side thought - why am I calling the subscription method? Shouldn't it just be called once on mounting the component, or when changing the conversation ID? Seems like calling it after each message creation is double the work.
**Link to work:** [Chatterson-Chatapp](https://github.com/kirbycampbell/chatterson-chatapp)

###################################################################################################

### Day 74 : May 27, 2019

**Today's Progress**: Worked about 7 hours, but slowly. Added React Router to the homepage app. It was simpler than I made it at first. Built it out with history.push syntax, and had tons of issues with it "POP"ing too much on "back" clicks. Switched to Link to components, and it worked like a charm. Began trying to add the "Skip the intro" function that will just render the page if you've already visited it.
**Thoughts:** : Gotta figure out a simpler way to alter the entrance sequence. Perhaps, I just set the program to automatically open to the main (end animation) view. Then if a user hasn't visited the site before, it loads the entrance sequence. Also, perhaps putting the main contents in a /main route would make it render if the browser goes back to that view, and the page only loads the animations if it starts on "/" proper. That could be an interesting way, That way people still get animations when revisiting, but don't get the animation when "back"ing up into the homepage. Idk, is this useless functionality for my home page? I feel like it isn't since pressing "back" is pretty usual functionality, would be pretty weird to reload the animation each time. We'll see tomorrow.
**Link to work:** [Homepage](https://github.com/kirbycampbell/homepage)

###################################################################################################

### Day 75 : May 28, 2019

**Today's Progress**: Got responsive mobile layout for resume section of homepage. Messed up the desktop resume layout at the same time, and attempted to fix alot of it.
**Thoughts:** : I'm trying to avoid using the javascript media query like i used in the original resume app, but i'm starting to think it would be more useful to go that direction. For now, I was just trying to rearrange the jsx to render in the correct order on mobile in a single column view, and still render the left/right column layout correctly for the desktop view. Mobile looks good now, but the desktop view is out of order, and I tried a few different ways of putting it back in order. Will figure out tomorrow!
**Link to work:** [Homepage](https://github.com/kirbycampbell/homepage)

###################################################################################################

### Day 76 : May 29, 2019

**Today's Progress**: Fixed responsive layout of resume and blog from homepage app. Added lots of material to the bio section. Cleaned up some layout stuff all over the homepage.
**Thoughts:** : Was a nice flow of fixing a bunch of small little bugs today on homepage. I obviously always want to do more in a day, but I'm feeling pretty CLOSE TO FINISHED with the homepage app. I mainly need to get the main entrance to only appear when you first visit, and never again. And I need to finish the bio page. Otherwise, this thing is nearly done!
**Link to work:** [Homepage](https://github.com/kirbycampbell/homepage)

###################################################################################################

### Day 77 : May 30, 2019

**Today's Progress**: Restructured the code to be much more organized in my store-front vintage app. I created specific files for filtered views, like page, and product pages. As well as setting up the structure for a cart page and more.
**Thoughts:** : This was a short little hour of coding, but tomorrow will be so much more! I've got a lot to knock out before my meeting at 1 to get the resume worked out!
**Link to work:** [Vintage Store-Front App](https://github.com/kirbycampbell/store-front)

###################################################################################################

### Day 78 : May 31, 2019

**Today's Progress**: Built a printable version of the resume app. Updated data in both resume app and homepage app. Tweaked some styling.
**Thoughts:** : Another sort of short coding day, but it was a busy day nonetheless. Tomorrow's going to be an amazing one!  
TODO for tomorrow:
-make resume projects clickable and linked to projects
-move all projects over to aws from heroku
-Finish the bio page of homepage app
-Add some styling to sign in and Sign up in Chat App.
-Avoid rendering "self" in the Chat App Friend List.

- Place a print button on the Resume pages.
  -Make homepage '/resume' routes externally link to the correct page. Right now it only works for a back button.
- Also similar note to last one - The active class on the Selection bar doesn't follow the back button route changes.
- whew thats a lot to do!
- ALSO UPDATE MY GITHUB README.md's for my main portfolio projects ahh!
  **Link to work:** [KirbyResume](https://github.com/kirbycampbell/kirby-resume)

###################################################################################################

### Day 79 : June 1, 2019

**Today's Progress**: Did SO much today. Knocked out 70% of the todo list from yesterday, which is surprising seeing how much there was. Sooo - I began by fixing style aspects of the homepage app. Then I moved all of portfolio apps over to aws. Then I fixed the jkirbycampbell.com nameservers issues, and got the homepage correctly connected to it (although on the west coast its going to take 40 more hours til it updates). Then I added a pdf link to the resume. Then I entered the Chat App zone - I fixed the API key again, but this time on the hosted version. Then I fixed the sign in and sign up buttons and the forms for each. I then restyled the landing page for chat app, so that it rendered a welcome message, and no friends list. I also filtered the "self" user out of the friends list, so you can no longer message yourself, which is probably good. I also completely overhauled the responsive layout view, and added the friend burger and friend over lay back!
**Thoughts:** : WHEW. Long one, but amazing stuff accomplished today. I think the end is in sight and its really making me clean up the last few/most obvious issues remaining. Not adding too many new features lately, but the last 10% of any project is so hard to complete actually, so many moving pieces, and you just want that clean cohesive look. I feel like I've been in style land (aka css) for longer than I'd really want to be. I just want my portfolio projects to look great, as well as act great.
Goals for tomorrow:
-Make the Tic Hack Joe app hard again - its too easy now.
-Hit the Todos for the Routes on Homepage app and active bar box.
-Add react native code to the portfolio section
-Add the code from the VR app

- Should probably build a c++ app for fun to add to portfolio too
  -Once those new domains are live, add those to the resume and portfolio links
  -Add Product page to vintage store app
  **Link to work:** [KirbyResume](https://github.com/kirbycampbell/kirby-resume)
  **Link to work2:** [Chatterson-Chatapp](https://github.com/kirbycampbell/chatterson-chatapp)

###################################################################################################

### Day 80 : June 2, 2019

**Today's Progress**: Another big one. Fixed the Routes on homepage app. First I bypassed the intro site animations, and just got the routes reorganized with the outer layout, and the inner sections. That took a bit, since the portfolio, blog, bio, and resume were all within the outer box. So I got the X button pushing history, and I am passing the history around to the components to properly have them render styles and fade outs with the back button changes. Then I added the initial animations back, which required complete code overhaul in the app.js functions and lots of changes within the titles.js, mainboxes.js, and socialbuttons.js (or whatever they are called, something close to that.). I also created a bunch of special hosted zones on aws route 53, copied nameservers around getting them linked with jkirbycampbell.com. I also tried just creating subdomains through AWS amplify, and I think I like the way that one works more thna the nameserver hosted zone way. Regardless, it was awesome to figure it out. I also got the direct route requests working on the homepage app, as AWS initially tried to render it server side, I had to cause a redirect that allows the React Router to work properly. Oh, and if you visited the site before the initial animations don't play, they only play on your first visit. Added that as a localStorage feature.
**Thoughts:** : This was a big one! Pretty self explainatory up there. Of course I continued my todo list from 2 days ago, and not the one I made last night... BUT... I pretty much 100% knocked out everything on the todo list from the night before, and obviously I had left the biggest items for last (the route fixes and aws subdomain hosting with routes). Feeling super accomplished, really feeling comfortable with this web coding stuff! My own big note on the homepage app is that I need to fix the localStorage function. I'm not sure I actually like the functionality of the app loading a different way on returning to the site. I think all links should open externally, and you should get the full animation everytime you enter the site from the outside/refresh the page. But I'd still like for the /resume /portfolio /blog /bio to load directly to their own pages, but just still including the animation on top. This might be relatively easy actually. Also I need to check that the blog links work now that I added the redirects.
**Link to work:** [Homepage](https://github.com/kirbycampbell/homepage)

###################################################################################################

### Day 81 : June 3, 2019

**Today's Progress**: Quick coding day. Began work on the news site's responsive mobile layout in Vue.js. Re organized the vue files for responsive layout, and also cleaned up the project file by getting rid of stuff I wasn't needing.
**Thoughts:** : A bit tired today, but I'm glad I started on this one! Hopefully I'll finish it tomorrow, even though I've got a pretty busy day ahead of me!  
**Link to work:** [JournalApp](https://github.com/kirbycampbell/journalapp)

###################################################################################################

### Day 82 : June 4, 2019

**Today's Progress**: Experimented in a local project with C++ linked lists and virtual pointers. Made a slight correction in the meditation app as well, since its hosted currently, didn't want to leave it live with that big bug.
**Thoughts:** : I'm really starting to understand the linked lists and virtual pointer's purpose for memory management in C++. It really makes me excited for designing super "clean" code, unlike the way I code in Javascript. They should call javascript the "just make it happen" language, where c++ is the "olympic coach" of coding languages. Gotta keep it tight!  
**Link to work:** [Local C++ Project] (No link today sorry!))

###################################################################################################

### Day 83 : June 5, 2019

**Today's Progress**: Continued building out a side c++ project to solidify my linked lists and virtual pointers knowledge. Artist managament system
**Thoughts:** : Still trying to break through on this linked lists and virtual pointers situation. I'm not sure where else to go with it, but I plan to break through today.
**Link to work:** [Artist Management C++](https://github.com/kirbycampbell/LinkedListOverloadExperiments)

###################################################################################################

### Day 84 : June 6, 2019

**Today's Progress**: Got most of this c++ experiment working. Artist app is working, dog breed one is having memory leaks, when I dive in deep.
**Thoughts:** : Probably coded for 13 hours today, no time to really write to 100-days-of-code because I'm so deep in the code itself lol. I guess thats the goal of 100DOC
**Link to work:** [Artist Management C++](https://github.com/kirbycampbell/LinkedListOverloadExperiments)

###################################################################################################

### Day 85 : June 7, 2019

**Today's Progress**: Another super long coding day. Finished some Linked Lists, Destructors, Deep Copy c++ projects. Also added project links to the resume and homepage-resume apps so that the boxes link to the appropriate AWS hosted domain pages. It's live!
**Thoughts:** : Still have some cleaning up to do on each app, and I could definitely use to add a link to the githubs for all of my FlatIron projects that showcase backends, jquery, rails/ruby, and more. I'm missing that content for sure. Hopefully tomorrow should be a bit less busy so I can put in more portfolio proper time, instead of the c++ stuff, although, I can definitely add some c++ to my portfolio, wouldn't hurt!
**Link to work:** [Homepage](https://github.com/kirbycampbell/homepage)

###################################################################################################

### Day 86 : June 8, 2019

**Today's Progress**: Returned to BlogCreator to fix some styling in the app. Began overhauling the toolbar into graphic/icon based toolbar, away from a text filled button toolbar.
**Thoughts:** : Been super busy studying for my finals this week, even though I have coded tons in c++ this weekend. Today I snuck in an hour and a half of forward progress on my portfolio projects, since I can't leave them sitting for long!
**Link to work0:** [Blog-Site](https://github.com/kirbycampbell/blog-site)

###################################################################################################

### Day 87 : June 9, 2019

**Today's Progress**: Continued working on the BlogSite's toolbar and css layouts. Fixed the toolbar's sizing, and div set up. Added fontawesome icons to the toolbar, and added hover functionality to each button to show the explanations.
**Thoughts:** : Still busy, but I squeezed in about 2 hours of coding tonight - really liking the way this app is looking. I should add a dark mode to this app soon. I need to look into how to change all colors from one switch. Obviously I'll need to tie one or two classNames as the color for background, buttons, hovers, etc... - when the button gets clicked, those few classes change to another className of colors, and it cascades all throughout the app. It shouldn't be too hard since the .user-made className is essentially used everywhere for background colors and hovers.
**Link to work0:** [Blog-Site](https://github.com/kirbycampbell/blog-site)
