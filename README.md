# twitter-profile-follow-counter-bot
This twitter bot will automatically update your profile name with the amount of followers

## Getting Started

### Prerequisites

#### Python

You need the following installed before you begin

```
Python 3.7
Pip
```

#### Twitter API Authentication

**Step 1:** Apply for a Twitter dev account

Next step is to create the Twitter API credentials from the [Twitter Developer site](https://developer.twitter.com/). Here, you have to select the Twitter user responsible for this account. It should probably be you or your organization.

**Step 2:** Create an Application

Twitter grants authentication credentials to apps, not accounts. An app can be any tool or bot that uses the Twitter API. So you need to register your an app to be able to make API calls.

To register your app, go to [your Twitter apps page](https://developer.twitter.com/en/apps) and select the Create an app option.

You need to provide the following information about your app and its purpose:

App name: a name to identify your application (such as examplebot)
Application description: the purpose of your application
Your or your application’s website URL: required, but can be your personal site’s URL since bots don’t need a URL to work
Use of the app: how users will use your app

**Step 3:** Create the Authentication Credentials

To create the authentication credentials, go to your [Twitter apps page](https://developer.twitter.com/en/apps) again.
Here you’ll find the Details button of your app. Clicking this button takes you to the next page, where you can generate the credentials.

By selecting the Keys and tokens tab, you can generate and copy the key, token, and secrets to use them in your code

**Step 4:** Export authentication credentials in your environment

In your .zshenv or .bash_profile export the credentials you acquired in step 3 e.g.

```
export CONSUMER_KEY="xxx"
export CONSUMER_SECRET="xxx"
export ACCESS_TOKEN="xxx"
export ACCESS_TOKEN_SECRET="xxx"
```

### Installing tweepy including dependencies

You can use a virtualenv offcourse (not neccesary). Begin by installing the required dependencies using pip in the root of this repository:

```
pip install -r requirements.txt
```

## Running the bot

If you exported the API credentials succesfully you can run the bot by:

```
python update_profile_follow_counter.py
```

## Authors

* **Danny Steenman** - *Initial work* - [dsteenman](https://github.com/dsteenman)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
