# KHAN-MD WhatsApp Bot

## Overview
KHAN-MD is a WhatsApp multi-device bot built with Node.js using the Baileys library. It provides various automation features for WhatsApp including auto-responses, message management, media downloads, and more.

## Project Structure
- `index.js` - Main entry point (obfuscated)
- `config.js` - Configuration settings
- `command.js` - Command utilities
- `app.json` - Heroku deployment configuration
- `package.json` - Node.js dependencies

## Running the Bot
The bot runs on port 5000 with an Express server for health checks. When started without a SESSION_ID, it displays a QR code in the console for WhatsApp Web authentication.

## Configuration
Configuration is done through environment variables:

### Required
- `SESSION_ID` - WhatsApp session ID (obtain from pairing service)

### Optional
- `PORT` - Server port (default: 5000)
- `BOT_NAME` - Bot display name
- `OWNER_NUMBER` - Owner's WhatsApp number
- `MODE` - Bot mode: public/private/group/inbox
- `PREFIX` - Command prefix (default: ".")

See `config.js` for all available options.

## System Dependencies
- ffmpeg - For media processing
- libwebp - For sticker creation

## Recent Changes
- 2026-01-25: Initial Replit setup, configured for port 5000

## User Preferences
- None recorded yet
