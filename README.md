# PcComponentes Outlet Bot

Receive a Telegram message when a graphics card is back to stock!
Currenly implemented for the outlet section of PcComponentes.com

New: Experimental automatic purchase available (no credit card needed) with adapted code from: https://github.com/elpatronaco/pccomponentes-buy-bot

> ⚠️ Disclaimer: Please note that this is a research project. I am by no means responsible for any usage of this tool. Use it on your behalf.

---

## Requirements

You will need Node.js and a node global package installed in your environement. Yarn is recommended as a package manager and script runner over npm.

### Node and npm

- #### Node installation on Windows

  Just go on [official Node.js website](https://nodejs.org/) and download the installer.
  Also, be sure to have `git` available in your PATH, `npm` might need it (You can find git [here](https://git-scm.com/)).

- #### Node installation on Ubuntu

  You can install nodejs and npm easily with apt install, just run the following commands.

  $ sudo apt install nodejs
  $ sudo apt install npm

- #### Other Operating Systems

  You can find more information about the installation on the [official Node.js website](https://nodejs.org/) and the [official NPM website](https://npmjs.org/).

If the installation was successful, you should be able to run the following command.

    $ node --version
    v14.16.1

    $ npm --version
    7.12.0

If you need to update `npm`, you can make it using `npm`! Cool right? After running the following command, just open again the command line and be happy.

    $ npm install npm -g

### Yarn

You can install yarn after installing npm with the following command.

    $ npm install --global yarn

If the installation was successful, you should be able to run the following command.

    $ yarn --version
    1.22.10

---

## Install

    $ git clone https://github.com/joanroig/pcalerts
    $ cd pcalerts
    $ yarn

## Configure app

Open the `config.json` file, then edit it with your settings.
Open the `.env` file in the root folder, change the BOT_TOKEN and CHAT_ID strings to connect your Telegram account:

- The BOT_TOKEN is provided by https://t.me/botfather, more info here: https://core.telegram.org/bots/api
- The CHAT_ID is provided after starting a chat with the Telegram bot.

If using the Purchase branch, also add those strings in the .env file with your account:

    PCC_USER=username@mail.com
    PCC_PASS=userpassword

## Running the project

    $ yarn start

Or easier if using a Raspberry (maybe chmod + x is needed), double click: `run_raspberry.sh`
