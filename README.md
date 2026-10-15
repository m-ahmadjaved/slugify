# Slugify — Discord URL Shortener Bot

A Node.js Discord bot that generates and manages shortened URLs directly in-server. Communities get fast, shareable links without ever leaving Discord.

![Status](https://img.shields.io/badge/status-complete-brightgreen)
![Node.js](https://img.shields.io/badge/runtime-Node.js-green)
![Discord.js](https://img.shields.io/badge/library-Discord.js-blue)

## The Problem

Sharing long URLs in Discord breaks the conversation flow. Existing URL shorteners require users to leave Discord, open a browser, and paste the link elsewhere — losing context and disrupting chat.

## The Solution

Slugify is a Discord bot that shortens URLs on the spot. Type a command in any channel, get a clean short link back — no tab switching, no external tools.

## Features

- **Custom command handler** — structured command parsing, easy to extend
- **URL shortening** — generates short, memorable slugs for any URL
- **Persistent storage** — link mappings saved to MongoDB
- **In-server workflow** — no leaving Discord required
- **Clean responses** — short links posted directly to the channel

## Tech Stack

| Layer | Technology |
|-------|------------|
| Runtime | Node.js |
| Bot Framework | Discord.js |
| Database | MongoDB |
| Persistence | Mongoose |

## Project Structure

```
slugify/
├── model/            # Mongoose schemas
├── index.js          # Bot entry point
├── server.js         # Express server (optional web endpoint)
├── package.json      # Dependencies and scripts
└── README.md         # This file
```

## Getting Started

### Prerequisites

- Node.js (v18+)
- MongoDB (local or Atlas)
- A Discord bot token ([how to create one](https://discord.com/developers/applications))

### Setup

```bash
git clone https://github.com/m-ahmadjaved/slugify.git
cd slugify
npm install
```

### Configuration

Create a `.env` file in the root:

```env
DISCORD_TOKEN=your_bot_token_here
MONGO_URI=mongodb://localhost:27017/slugify
```

### Run

```bash
npm start
```

The bot will connect to Discord and be ready to receive commands.

## Author

**Muhammad Ahmad Javed**
BS Computer Science (Hons.), University of Agriculture, Faisalabad

- Portfolio: [imahmad.xyz](https://imahmad.xyz)
- GitHub: [@m-ahmadjaved](https://github.com/m-ahmadjaved)
- LinkedIn: [m-ahmadjaved](https://linkedin.com/in/m-ahmadjaved)
