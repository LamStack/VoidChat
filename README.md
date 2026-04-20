# VoidChat 🌑

A modern, real-time multimedia chat application built with Firebase. Supports text, image, and audio messaging across multiple channels with a clean, responsive interface.

## 🚀 Features

### Core Messaging
- **Real-time Text Chat** — Instant messaging with live updates
- **Image Sharing** — Upload and share images with built-in compression tools
- **Audio Recording** — Record audio messages directly in the browser
- **Emoji Reactions** — Add reactions to messages (❤️, 👍, 😂, 😮, 🔥, 👏, 💯, 🎉)

### Multi-Channel Support
- **#general** — Main discussion channel
- **#media-share** — Dedicated channel for media sharing
- **#random** — Off-topic conversations
- **Unread Badges** — Visual indicators for new messages in other channels
- **Instant Switching** — Switch between channels without losing context

### User Experience
- **Online Presence** — Live user count and avatar previews in the top bar
- **Typing Indicators** — See when others are typing in real-time
- **User Avatars** — Choose from 6 emoji avatars (🧑, 👩, 🧔, 👨‍💻, 👩‍💻, 🧑‍🎓)
- **Toast Notifications** — Brief notifications for events like joining or image processing
- **Responsive Design** — Optimized for desktop and mobile devices
- **Mobile Sidebar** — Hamburger menu (☰) to toggle sidebar on small screens

### Image Processing Tools
- **Quality Compression** — Adjust JPEG quality from 1-100%
- **Format Conversion** — Convert images to JPEG, PNG, or WebP
- **Size Preview** — See original vs. compressed file sizes before uploading
- **Lightbox Viewer** — Click images to view them in full-screen overlay

### Audio Features
- **Browser Recording** — Record audio using the device's microphone
- **Waveform Visualization** — Animated waveform during playback
- **Duration Display** — Shows recording/playback time
- **Simulated Audio** — Fallback for devices without microphone access

### Session Management
- **Auto-Clear History** — Chat history is cleared when the browser tab is closed
- **Presence Tracking** — Users are automatically removed from online list on disconnect
- **Typing Cleanup** — Typing indicators are cleaned up on disconnect

## 🛠 Tech Stack

- **Frontend**: HTML5, CSS3, Vanilla JavaScript (ES6+)
- **Backend**: Firebase Realtime Database
- **Styling**: Custom CSS with CSS Variables for theming
- **Icons**: Unicode emojis and symbols
- **Audio**: Web Audio API and MediaRecorder API
- **Images**: Canvas API for compression and format conversion

## 📱 Mobile Support

VoidChat is fully responsive and works on iPhone and Android devices:

- **Touch-Friendly UI** — Larger buttons and touch targets
- **Mobile Meta Tags** — Enables full-screen web app mode
- **Sidebar Toggle** — Hamburger menu for accessing channels and users
- **Optimized Layout** — Adjusted padding, fonts, and spacing for small screens

## 🚀 Getting Started

### Prerequisites
- Modern web browser with JavaScript enabled
- Internet connection for Firebase connectivity
- Microphone access (optional, for audio recording)

### Installation

1. **Clone or Download the Repository**
   ```
   git clone https://github.com/yourusername/VoidChat.git
   cd VoidChat
   ```

2. **Open the Application**
   - Open `index.html` in your web browser
   - No server setup required - it's a client-side application

### Usage

1. **Join the Chat**
   - Select an avatar emoji from the 6 options
   - Enter your display name (maximum 20 characters)
   - Click "Join Chat →" to connect

2. **Start Messaging**
   - Type messages in the input box at the bottom
   - Press Enter or click the send button (➤) to send
   - Use Shift+Enter for multi-line messages

3. **Share Images**
   - Click the "🖼 Image" button to select an image file
   - Optionally add a caption
   - Use the compression tools to optimize file size
   - Click "Apply ✓" to process, then send

4. **Record Audio**
   - Click the "🎙 Record" button to start recording
   - Click "⏹ Stop" to finish
   - The audio message will be sent automatically

5. **React to Messages**
   - Hover over any message to see the "+ 😊" button
   - Click to open emoji picker and select a reaction

6. **Switch Channels**
   - Click channel names in the sidebar (#general, #media-share, #random)
   - Unread message counts appear as badges

7. **Mobile Usage**
   - On small screens, click the hamburger menu (☰) to open the sidebar
   - Tap outside the sidebar to close it

## 🎨 Customization

### Theming
The app uses CSS custom properties (variables) for easy theming:

```css
:root {
  --bg: #f5f4f0;           /* Background color */
  --surface: #fff;         /* Card/surface color */
  --surface2: #f0efe9;     /* Secondary surface */
  --border: rgba(0,0,0,0.08);  /* Border color */
  --text: #1a1a1a;         /* Primary text */
  --accent: #2563eb;       /* Accent color (blue) */
  --green: #16a34a;        /* Success color */
  --red: #dc2626;          /* Error color */
}
```

### Adding More Channels
To add new channels, update the HTML in the sidebar section and add corresponding JavaScript logic.

### Custom Emojis
Add more reaction emojis by updating the `showEmojiPick` function in the JavaScript.

## 🔧 Firebase Configuration

The app is pre-configured with a Firebase project. To use your own:

1. Create a Firebase project at https://console.firebase.google.com/
2. Enable Realtime Database
3. Update the `firebaseConfig` object in `index.html` with your credentials
4. Set database rules to allow read/write access

## 📂 Project Structure

```
VoidChat/
├── index.html          # Main application file
├── README.md           # This file
└── (no other files)    # Single-file application
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- Built for ITCE436 course project
- Uses Firebase for real-time database functionality
- Icons and emojis from Unicode standard
- Inspired by modern chat applications like Discord and Slack

## 🐛 Known Issues

- Audio recording requires microphone permissions
- Large images may take time to compress
- Browser compatibility: Requires modern browsers with ES6 support
- Mobile browsers may have limitations with audio recording

## 📞 Support

For questions or issues, please open an issue on the GitHub repository.

---

**VoidChat 🌑** - Real-time multimedia communication made simple.
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

