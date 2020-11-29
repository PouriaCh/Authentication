# Secrets
Secrets is a Node.js app that allows the users to submit their secrets anonymously! It means your identity would never be revealed to the public and only your secrets will be listed along with everybody else's. Give it a try and let me know!

## Getting Started
1. Clone the repository by:

```
git clone https://github.com/PouriaCh/Secrets-with-Website-Authentication.git
```

2. Make sure you have installed <a href="https://nodejs.org/en/download/">Node.js</a> in your local machine.

3. Go to the main folder of the repository and run the following command:

```
npm install
```

This will make sure that you install all the required modules listed in <i>package.json</i>.

4. This app integrates Open Authentication (OAuth) for Google, Facebook, and GitHub users. The middleware that we use for authentication is <a href="http://www.passportjs.org/">Passport.js</a> which offers simple authentication for Node.js apps.

You need to include Google, Facebook and GitHub strategies for OAuth purposes. Check out the following links:

<ul>
  <li><a href="http://www.passportjs.org/packages/passport-google-oauth20/">passport-google-oauth20</a></li>
  <li><a href="http://www.passportjs.org/packages/passport-facebook/">passport-facebook</a></li>
  <li><a href="http://www.passportjs.org/packages/passport-github2/">passport-github2</a></li>
</ul>

Follow the instructions step-by-step according to these links.

5. Create a file named <code>.env</code> inside the main folder of the project. You need to copy your <code>CLIENT_ID</code> and <code>CLIENT_SECRET</code> for each strategy mentioned above. Something like:

```
SECRET=thisisourlittlesecret.
SESSION_SECRET=Our little secret.
GOOGLE_CLIENT_ID=...
GOOGLE_CLIENT_SECRET=...
FACEBOOK_APP_ID=...
FACEBOOK_APP_SECRET=...
GITHUB_CLIENT_ID=...
GITHUB_CLIENT_SECRET=...
```

Instead of <code>...</code>, insert your own data from the Developer Console of Google, Facebook, and GitHub (without any , or "" or space). Make sure your <code>.env</code> is listed inside the <code>.gitignore</code> file in case you want to push your work to GitHub.
