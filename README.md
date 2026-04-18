# VoidChat 🌑

A modern, real-time multimedia chat application with text, image, and audio messaging capabilities. Built for ITCE436 course project.

## Features

### Core Messaging
- **Text Messages** — Real-time text chat with emoji reactions
- **Image Sharing** — Share images with built-in compression and format conversion (JPEG, PNG, WebP)
- **Audio Recording** — Record and share audio messages directly in the chat
- **Emoji Reactions** — React to messages with emojis

### Multi-Channel Support
- **#general** — Main discussion channel
- **#media-share** — Media-focused sharing channel
- **#random** — Off-topic conversations
- Real-time channel switching with unread badge counts

### User Experience
- **Online Presence** — See who's online with live user count and avatar preview
- **Typing Indicators** — Know when others are typing
- **User Avatars** — Choose from 6 emoji avatars on join
- **Notifications** — Toast notifications for events
- **Responsive Design** — Works on desktop and mobile (hides sidebar on mobile)

### Image Tools
- **Compression** — Adjust JPEG quality (1-100%)
- **Format Conversion** — Convert between JPEG, PNG, and WebP
- **Size Preview** — See file size savings before uploading

## Tech Stack

- **Frontend** — HTML5, CSS3, Vanilla JavaScript
- **Backend** — Firebase Realtime Database
- **UI** — Custom CSS with CSS variables for theming
- **Icons** — Emojis and Unicode symbols

## Getting Started

1. **Open the application**
   ```
   Open VoidChat.html in a modern web browser
   ```

2. **Join the chat**
   - Select an avatar emoji
   - Enter your name (max 20 characters)
   - Click "Join Chat" to connect

3. **Start chatting**
   - Switch between channels using the sidebar
   - Type messages and press Enter or click the Send button
   - Use image/audio buttons to share media
   - Click reaction buttons to add emoji reactions to messages

## Features Breakdown

### Messaging
- **Text:** Type in the input box and press Enter or click Send
- **Images:** Click 🖼 Image button, select a file, optionally compress/convert, then send
- **Audio:** Click 🎙 Record button to start recording, stop to save and send
- **Emojis:** Quick emoji insert buttons or full emoji reactions on messages

### Channels
- Switch channels via the sidebar (desktop) or menu (mobile)
- Each channel shows unread message count in badges
- Channel descriptions appear in the chat header

### User Management
- Real-time online user list with green dot indicators
- Avatars shown for each message
- Own messages appear on the right with blue bubble
- Other messages appear on the left with gray bubble

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)

## Notes

- Requires internet connection for Firebase synchronization
- User data stored in Firebase Realtime Database
- Messages persist as long as Firebase project is active
- Audio and image data stored with messages

## Author

Built for ITCE436 course project

