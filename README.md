## Getting Started
-   Create a `.env` file in the root directory and store the following:
    -   MONGO_URI=Insert the correct connection URL for your MongoDB database
    -   REACT_APP_GOOGLE_CLIENT_ID=Insert the valid google client id
    -   REACT_APP_TWIITER_CONSUMER_ID=Insert the valid twitter consumer id
    -   REACT_APP_TWITTER_CONSUMER_SECRET=Insert the valid twitter consumer id
-   Run the server on PORT 5000
-   npm start/yarn start

You can obtain the MONGO_URI after create a collectoin on [mongodb atlas](https://www.mongodb.com/cloud/atlas). For the GOOGLE_CLIENT_ID and the TWITTER_CONSUMER_SECRET/ID, you will need to go through the Google developer console and the Twitter developer accounts page respectively

## Info

-   This is a blogging PWA with user authentication and authorization. There is also a social login option, to login using your Twitter or Google accounts. The blog posts are displayed in the reverse chronological order by default.
-   There is no exploitation of data, as the app only requires access to your accounts to fetch your unique ID for authentication/authorization purposes, and no personal details(except your registred user name on the social account) is used by the application.
-   The frontend of the app is built using React and I have used Bootstrap classes for styling the compnents in addition to my local CSS styles.
-   It is a blog app that lets users read the existing blog posts without logging in, and lets them share their thoughts using the anonymous comment section.
-   Each comment has a unique jdenticon icon to represent the user who commented anonymously
-   There is also a profanity filter to disallow usage of certain NSFW words in the comments' section. This is not an attempt to hinder freedom of speech, but instead it is a necessary aid to prevent misuse of the platform by nefarious users.
-   In order to write a new blog post, the user has to login using one of the social media login options provided. The react-social-login package is being used to provide the user authentication and authorization.