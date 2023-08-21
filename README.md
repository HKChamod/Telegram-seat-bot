# Telegram Lucky Number Bot

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [Features](#features)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This is a simple Telegram bot built using the `node-telegram-bot-api` library. The bot allows administrators of a group to generate lucky numbers for users. Each user can request a lucky number, and once all available lucky numbers are generated, no more numbers can be assigned.

## Prerequisites

- Node.js (v14 or higher)

## Installation

1. Clone the repository or download the code.
2. Install the required dependencies by running the following command in the project directory:

npm install


## Configuration

1. Open the `index.js` file.
2. Replace `'PAST-YOUR-TELEGRAM-BOT-API-HERE'` with your actual Telegram Bot API token.

## Usage

1. Start the bot by running the following command in the project directory:

node index.js


2. Add the bot to your Telegram group.
3. As an admin, send the `/start` command in the group chat to initialize the bot. Only admins can use this command.
4. The bot will send a welcome message with a button labeled "Get Your Lucky number". Users can click the button to request a lucky number.
5. Once all lucky numbers are generated (controlled by the `userCount` variable), no more numbers can be assigned.

## Features

- Admins can initiate the bot using the `/start` command.
- Users can request a lucky number using the button provided by the bot.
- Users are limited to one lucky number each.
- The bot prevents users from requesting more than one lucky number.
- The bot informs users when all lucky numbers have been generated.

## Contributing

Contributions are welcome! Feel free to open issues and submit pull requests for improvements or bug fixes.

## License

This project is licensed under the [MIT License](LICENSE).
