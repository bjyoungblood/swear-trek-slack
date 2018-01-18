# [Swear Trek](https://twitter.com/swear_trek) Slack Slash Command

## aka the new reason you're not getting your work done

![You're not getting your work done because](https://78.media.tumblr.com/8babd66c6cd3dd9b78c35bcf328fefbf/tumblr_p2i7f0kFMj1vaqoiqo1_400.gif)

## Installation

Do you really need installation instructions? Because

![Yes, I really need installation instructions](https://78.media.tumblr.com/7c967fdc5e76a66aab9ff0da90bec9f4/tumblr_p0pburEDsI1vaqoiqo1_540.gif)

### Fine, I'll tell you what to do

![You obviously need help](https://78.media.tumblr.com/fb9e76a55875e3487deb05ce0de3604f/tumblr_p2555szSB51vaqoiqo1_400.gif)

1. Create a Tumblr OAuth application
   1. Log into your Tumblr account (or make one)
   1. [Register an OAuth application](https://www.tumblr.com/oauth/apps)
     - Default callback URL doesn't really matter for this (you can use `http://localhost` if you want, but don't blame me if that's against the TOS)
   1. Take note of the `OAuth Consumer Key`
     - You don't need the consumer/secret key or anything else
1. PRESS THE PURPLE BUTTON, enter key you got from Tumblr, and take note of the name of the Heroku app

   [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)
1. Add a slash command to your Slack workspace using the following settings:
   - Command: `/sweartrek` probably makes sense
   - URL: `https://HEROKU_APP_NAME.herokuapp.com/slack`
     - Remember how you noted the name of your Heroku app above?
   - Method: `POST`
     - Not `GET`. `GET` won't work.
   - Other options: none of the other options matter (as of now), so customize to your heart's desire
1. Type `/sweartrek` (or the alternate command alias you picked) in Slack and enjoy

## Feature Requests

![yeah no maybe](https://78.media.tumblr.com/9e439c8d9f925aa808e309bd7e171303/tumblr_p0paqun0Ow1vaqoiqo1_400.gif)

Seriously though, if you have a cool idea, make a pull request. If you're not sure where to start, open an issue with your idea and questions, and I'll do my best to help you out!

## Troubleshooting

If you figured out the above steps, you can probably figure out how to get the Heroku logs. File an issue, and I (or another kind person) might help you out when there's time.
