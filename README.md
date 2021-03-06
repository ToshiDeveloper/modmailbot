
## What is Modmail?

Modmail is similar to Reddit's Modmail, both in functionality and purpose. It serves as a shared inbox for server staff to communicate with their users in a seamless way.

This bot is free for everyone and always will be. If you like this project and would like to show your appreciation, you can support us on **[Patreon](https://www.patreon.com/toshidev)**, cool benefits included! 

## How does it work?

When a member sends a direct message to the bot, Modmail will create a channel or "thread" into a designated category. All further DM messages will automatically relay to that channel; any available staff can respond within the channel.

Our Logviewer will save the threads so you can view previous threads through their corresponding log link. Here is an [**example**](https://logs.modmail.dev/example).

## Features

* **Highly Customisable:**
  * Bot activity, prefix, category, log channel, etc.
  * Command permission system.
  * Interface elements (color, responses, reactions, etc.).
  * Snippets and *command aliases*.
  * Minimum duration for accounts to be created before allowed to contact Modmail (`account_age`).
  * Minimum length for members to be in the guild before allowed to contact Modmail (`guild_age`). 

* **Advanced Logging Functionality:**
  * When you close a thread, Modmail will generate a [log link](https://logs.modmail.dev/example) and post it to your log channel.
  * Native Discord dark-mode feel.
  * Markdown/formatting support.
  * Login via Discord to protect your logs ([premium Patreon feature](https://www.patreon.com/toshidev)).
  * See past logs of a user with `?logs`.
  * Searchable by text queries using `?logs search`.

* **Robust implementation:**
  * Schedule tasks in human time, e.g. `?close in 2 hours silently`.
  * Editing and deleting messages are synced.
  * Support for the diverse range of message contents (multiple images, files).
  * Paginated commands interfaces via reactions.

This list is ever-growing thanks to active development and our exceptional contributors. See a full list of documented commands by using the `?help` command.

## Installation

Where can I find the Modmail bot invite link? 

Unfortunately, due to how this bot functions, it cannot be invited. The lack of an invite link is to ensure an individuality to your server and grant you full control over your bot and data. Nonetheless, you can quickly obtain a free copy of Modmail for your server by following one of the methods listed below (roughly takes 15 minutes of your time).

### Heroku

You can host this bot on Heroku.

Installation via Heroku is possible with your web browser alone. 
The [**installation guide**](https://github.com/kyb3r/modmail/wiki/Installation) (which includes a video tutorial!) will guide you through the entire installation process. If you run into any problems, join our [Modmail Discord Server](https://discord.gg/etJNHCQ) for help and support.

To configure automatic updates:
 - Login to [GitHub](https://github.com/) and verify your account.
 - [Fork the repo]().
 - Install the [Pull app](https://github.com/apps/pull) for your fork. 
 - Then go to the Deploy tab in your [Heroku account](https://dashboard.heroku.com/apps) of your bot app, select GitHub and connect your fork (usually by typing "Modmail"). 
 - Turn on auto-deploy for the `master` branch.

### Hosting for Patreons

If you don't want to go through the trouble of setting up your very own Modmail bot or wish to support this project, we got a solution for you! We offer the complete installation, hosting, and maintenance of your Modmail with [**Patreon**](https://www.patreon.com/toshidev). Join our [Modmail Discord Server](https://discord.gg/etJNHCQ) for more info! 

### Locally

Local hosting of Modmail is also possible. First, you will need [`Python 3.7`](https://www.python.org/downloads/release/python-376/).

Follow the [**installation guide**](https://github.com/kyb3r/modmail/wiki/Installation) and disregard deploying the Heroku bot application. If you run into any problems, join our [Modmail Discord Server](https://discord.gg/etJNHCQ) for help and support.

Clone the repo:

```console
$ git clone https://github.com/kyb3r/modmail
$ cd modmail
```

Install dependencies:

```console
$ pipenv install
```

Rename the `.env.example` to `.env` and fill out the fields. If `.env.example` is nonexistent (hidden), create a text file named `.env` and copy the contents of [`.env.example`](https://raw.githubusercontent.com/kyb3r/modmail/master/.env.example) then modify the values.

Finally, start Modmail.

```console
$ pipenv run bot
```

#### Docker

This repo supplies a Dockerfile for simplified deployment. 

You can build your own Docker image:

```console
$ docker build . --tag=modmail
```

Or run directly from a pre-built version from https://hub.docker.com/.

- Kyber's:

```console
$ docker pull kyb3rr/modmail
```

And to run your docker image:

```console
$ docker run --env-file .env kyb3rr/modmail
```
- `.env` should be the path to your env file; you can also supply a path: `/path/to/.env`.


## Plugins

Modmail supports the use of third-party plugins to extend or add functionalities to the bot.
Plugins allow niche features as well as anything else outside of the scope of the core functionality of Modmail. 

You can find a list of third-party plugins using the `?plugins registry`  command or visit the [Unofficial List of Plugins](https://github.com/kyb3r/modmail/wiki/Unofficial-List-of-Plugins) for a list of plugins contributed by the community.

To develop your own, check out the [plugins documentation](https://github.com/kyb3r/modmail/wiki/Plugins).

Plugins requests and support are available in our [Modmail Support Server](https://discord.gg/j5e9p8w).

## Contributing

Contributions to Modmail are always welcome, whether it be improvements to the documentation or new functionality, please feel free to make the change. Check out our [contributing guidelines](https://github.com/kyb3r/modmail/blob/master/.github/CONTRIBUTING.md) before you get started.

If you like this project and would like to show your appreciation, support us on **[Patreon](https://www.patreon.com/kyber)**!

