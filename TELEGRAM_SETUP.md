# Telegram Bot Setup Guide

## Step 1: Create a Telegram Bot

1. Open Telegram and search for `@BotFather`
2. Start a chat with BotFather
3. Send `/newbot` command
4. Follow the instructions to create your bot
5. Save the bot token (looks like: `7585922085:AAGNv_nYCCiNF4xv8H4lwJxaJC-y0QzPYgc`)
7585922085:AAGNv_nYCCiNF4xv8H4lwJxaJC-y0QzPYgc

## Step 2: Get Your Chat ID

### Method 1: Using @userinfobot
1. Search for `@userinfobot` in Telegram
2. Start a chat with it
3. It will send you your chat ID

### Method 2: Using your bot
1. Send a message to your bot
2. Visit: `https://api.telegram.org/bot<YOUR_BOT_TOKEN>/getUpdates`
3. Find your chat ID in the response

## Step 3: Configure the Bot

1. Open `js/script.js`
2. Find these lines (around line 115-116):
   ```javascript
   const BOT_TOKEN = 'YOUR_BOT_TOKEN_HERE'; // Replace with your bot token
   const CHAT_ID = 'YOUR_CHAT_ID_HERE'; // Replace with your chat ID
   ```
3. Replace with your actual values:
   ```javascript
   const BOT_TOKEN = '123456789:ABCdefGHIjklMNOpqrsTUVwxyz';
   const CHAT_ID = '123456789';
   ```

## Step 4: Test the Integration

1. Fill out any form on your website
2. Submit the form
3. Check your Telegram for the notification

## Features

- **Instant Notifications**: Get leads immediately in Telegram
- **Formatted Messages**: Clean, readable message format
- **Multiple Form Types**: Different message formats for contact vs consultation
- **Error Handling**: Shows success/error notifications to users
- **No Server Dependencies**: Works without PHP or email servers

## Message Format

The bot will send messages like:
```
🆕 Yangi Murojaat

👤 Ism: John Doe
📞 Telefon: +998901234567
📧 Email: john@example.com

⏰ Vaqt: 12/25/2023, 2:30:45 PM
🌐 Sahifa: https://yourwebsite.com
```

## Security Notes

- Keep your bot token private
- Consider using environment variables for production
- The bot token should not be exposed in client-side code for high-security applications
