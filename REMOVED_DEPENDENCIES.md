# Removed Dependencies

## PHP Mailer Files (No Longer Needed)

The following files have been replaced by Telegram Bot integration and can be safely removed:

### Files to Remove:
- `bat/rd-mailform.php` - PHP mail form handler
- `bat/rd-mailform.config.json` - Mail form configuration
- `bat/rd-mailform.tpl` - Mail form template
- `bat/reCaptcha.php` - reCaptcha verification
- `bat/ReCaptcha/` - reCaptcha library directory
- `bat/phpmailer/` - PHPMailer library directory

### Why Removed:
- **No Server Dependencies**: Telegram bot works without PHP or email servers
- **Instant Notifications**: Get leads immediately in Telegram
- **Better Reliability**: No email delivery issues or server downtime
- **Simplified Setup**: No need to configure email servers or PHP mail settings

### Benefits:
1. **Faster Loading**: No PHP processing required
2. **Better Security**: No server-side code execution
3. **Easier Deployment**: Works on any static hosting
4. **Instant Feedback**: Real-time notifications in Telegram
5. **No Email Spam**: Direct messaging instead of email

### What's New:
- Telegram Bot integration in `js/script.js`
- Form handling via JavaScript/jQuery
- Instant notifications with success/error messages
- Clean, formatted messages in Uzbek language

## Next Steps:
1. Follow the `TELEGRAM_SETUP.md` guide to configure your bot
2. Test the forms to ensure they work correctly
3. Remove the PHP files if you want to clean up the project
4. Consider moving to WordPress for easier content management
