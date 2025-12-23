# HelpNearby 🌱

A beautiful, real-time community help platform where people can post and respond to help requests in their local area.

![HelpNearby Banner](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)
![Firebase](https://img.shields.io/badge/Firebase-v10.7.1-orange?style=for-the-badge&logo=firebase)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

## ✨ Features

- 📝 **Post Help Requests** - Ask for help with studies, travel, tech issues, or anything else
- 🎯 **Category Filtering** - Filter requests by category (Notes/Study, Guidance, Travel, Tech Help, Other)
- 📍 **Location-Based** - Specify your location so people nearby can help
- ❤️ **Helper Counter** - See how many people are willing to help with each request
- 🌓 **Dark Mode** - Beautiful light and dark themes
- ⚡ **Real-Time Updates** - Powered by Firebase Firestore for instant updates
- 📱 **Responsive Design** - Works seamlessly on desktop, tablet, and mobile
- 🎨 **Modern UI** - Stunning gradients, smooth animations, and glass-morphism effects

## 🚀 Quick Start

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- Internet connection (for Firebase)

### Installation

1. **Clone or download this repository**
   ```bash
   git clone https://github.com/yourusername/helpnearby.git
   cd helpnearby
   ```

2. **Open the HTML file**
   - Simply open `index.html` in your web browser
   - No build process or server required!

3. **Start using**
   - Post your first help request
   - Toggle between light and dark modes
   - Filter requests by category

## 🔧 Configuration

The app is already configured with Firebase. If you want to use your own Firebase project:

1. Create a new Firebase project at [Firebase Console](https://console.firebase.google.com/)

2. Enable Firestore Database in your Firebase project

3. Replace the Firebase configuration in the HTML file:
   ```javascript
   const firebaseConfig = {
       apiKey: "YOUR_API_KEY",
       authDomain: "YOUR_AUTH_DOMAIN",
       projectId: "YOUR_PROJECT_ID",
       storageBucket: "YOUR_STORAGE_BUCKET",
       messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
       appId: "YOUR_APP_ID",
       measurementId: "YOUR_MEASUREMENT_ID"
   };
   ```

4. Set up Firestore security rules:
   ```javascript
   rules_version = '2';
   service cloud.firestore {
     match /databases/{database}/documents {
       match /helps/{helpId} {
         allow read: if true;
         allow create: if true;
         allow update: if true;
       }
     }
   }
   ```

## 📖 Usage

### Posting a Help Request

1. Select a category from the dropdown (📚 Notes/Study, 🧭 Guidance, etc.)
2. Enter your location (e.g., "Campus Library, Block A")
3. Describe what help you need (max 200 characters)
4. Click "📤 Post Request"

### Helping Others

1. Browse through the help requests
2. Use the filter to find requests in specific categories
3. Click "I can help!" on any request you can assist with
4. The helper counter will increment to show your support

### Dark Mode

- Click the 🌙/☀️ button in the top-right corner to toggle between light and dark themes

## 🎨 Categories

- 📚 **Notes / Study** - Academic help, study materials, notes sharing
- 🧭 **Guidance** - Career advice, mentorship, direction
- 🚌 **Travel / Local** - Local navigation, travel tips, directions
- 💻 **Tech Help** - Technology issues, software help, debugging
- 🤝 **Other** - Anything else you need help with

## 🛠️ Technology Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Database**: Firebase Firestore (NoSQL, Real-time)
- **Fonts**: Google Fonts (Poppins)
- **Hosting**: Can be deployed anywhere (GitHub Pages, Netlify, Vercel, etc.)

## 📱 Browser Support

- ✅ Chrome (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Opera

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Create a Pull Request

## 📝 Future Enhancements

- [ ] User authentication and profiles
- [ ] Direct messaging between helper and requester
- [ ] Push notifications for new requests
- [ ] Map view for location-based requests
- [ ] Request expiration/auto-close after 24 hours
- [ ] Rating system for helpers
- [ ] Image attachments for requests
- [ ] Search functionality

## 🐛 Known Issues

- None at the moment! Report issues on GitHub.

## 📄 License

This project is licensed under the MIT License - see below for details:

```
MIT License

Copyright (c) 2025 HelpNearby

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## 👨‍💻 Developer

Made with ❤️ by Kartik, Alhaj(leader), Aanchal

## 🙏 Acknowledgments

- Firebase for the real-time database
- Google Fonts for the beautiful Poppins font
- The open-source community for inspiration

---

**Need help?** Open an issue on GitHub or reach out to the community!

**Love the project?** Give it a ⭐ on GitHub!
