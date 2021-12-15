# Leaderboard

> In this activity you will set up a JavaScript project for the Leaderboard list app, using webpack and ES6 features, notably modules. You should develop a first working version of the app following a wireframe, but without styling - just focus on functionality. In following activities, you will consume the Leaderboard API using JavaScript async and await and add some styling.

## Screenshots:

![screenshot](https://github.com/mohamedelshamy55/Leaderboard/blob/setup-project/screenshot.png)


Porject's features are added into seperate branch to keep main branch safe.

## Built With

- Major languages (HTML, CSS, JavaScript)
- Frameworks (None)
- Technologies used
- Webpack(Code Bundlng et al)
- Git(version control)
- ESLint(JavaScript linting)
- WebHint(linting tool)
- Stylelint(style linting)

## Online live link

[Visit project online](https://github.com/mohamedelshamy55/Leaderboard)

## Getting Started

To get a local copy up and running follow these simple example steps.

### Using it Locally
Getting Started
To get a local copy up and running follow these simple example steps.

Prerequisites
A text editor(preferably Visual Studio Code)
Install
Git
Node
Usage
Clone this repository
$ gi clone https://github.com/mohamedelshamy55/Leaderboard.git
$ cd LeaderBoard
Run project
$ npm install
$ npm run start # this will make webpack watching for your changes in code
Open page in browser
$ open dist/index.html
Interaction with the leaderboard API
Each new game is created with the POST method using
    { 
        "name": "My cool new game" 
    }
This request returns a result that holds the unique ID for that game:

  {
    "result": "Game with ID: Zl4d7IVkemOTTVg2fUdz added."
  }
This gameID is saved in the localStorage automatically

The two allowed actions are psoting of scores and getting of the scores

The POST request creates a new Leaderboard score for the given game sending user and score as parameters like this:

Endpoint
https://us-central1-js-capstone-backend.cloudfunctions.net/api/games/:id/scores/
body parameters

{ 
    "user": "John Doe",
    "score": 42
}
and it returns

{
    "result": "Leaderboard score created correctly."
}
The GET request returns data in JSON format like this:

Endpoint
https://us-central1-js-capstone-backend.cloudfunctions.net/api/games/:id/scores/
It returns

{
  "result": [
      {
          "user": "John Doe",
          "score": 42
      },
      {
          "user": "Peter Parker",
          "score": 35
      },
      {
          "user": "Wonder Woman",
          "score": 50
      }
  ]
}

## Visit And Open Files

[Visit Repo](https://github.com/mohamedelshamy55/Leaderboard)

## Authors

👤 **MOHAMED ELSHAMY**

- GitHub: [@githubhandle](https://github.com/mohamedelshamy55)
- Twitter: [@twitterhandle](https://mobile.twitter.com/moelshamy55)
- LinkedIn: [LinkedIn](https://www.linkedin.com/in/mohamed-elshamy85/)

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

Feel free to check the [issues page](https://github.com/mohamedelshamy55/Leaderboard/issues).

## Show your support

Give a ⭐️ if you like this project!

## Acknowledgments

- Inspiration: Microverse

🤝 Contributing
Contributions, issues, and feature requests are welcome!

Show your support
Give a ⭐️ if you like this project!

Acknowledgments
Hat tip to anyone whose code was used
Inspiration
etc 📝 License This project is MIT licensed.
