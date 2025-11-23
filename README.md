# 🐕 VRM Desktop Assistant

<div align="center">

![VRM Desktop Assistant](https://img.shields.io/badge/VRM-Desktop%20Assistant-blue?style=for-the-badge&logo=3d&logoColor=white)
![Electron](https://img.shields.io/badge/Electron-191970?style=for-the-badge&logo=Electron&logoColor=white)
![Three.js](https://img.shields.io/badge/threejs-black?style=for-the-badge&logo=three.js&logoColor=white)
![AI Powered](https://img.shields.io/badge/AI-Powered-green?style=for-the-badge&logo=openai&logoColor=white)

*A cute, interactive 3D VRM character that lives on your desktop with AI chat capabilities!*

[Features](#-features) • [Installation](#-installation) • [Usage](#-usage) • [Configuration](#-configuration) • [Development](#-development)

</div>

---

## ✨ Features

### 🎯 Core Features
- **🐾 Interactive 3D VRM Character** - Beautiful VRM model rendering with Three.js
- **🧠 AI Chat Integration** - Smart conversations with OpenAI/OpenRouter APIs  
- **🎮 Desktop Companion** - Lives on your desktop, always ready to help
- **🎨 Customizable Appearance** - Transparency, positioning, and visual settings
- **💫 Smooth Animations** - Responsive character animations and movements
- **⚙️ Easy Configuration** - User-friendly settings panel

### 🤖 AI Capabilities
- **Conversational AI** - Friendly dog personality with enthusiasm and loyalty
- **Context Awareness** - Remembers conversation history for natural dialogue
- **Multiple AI Providers** - Support for both OpenAI and OpenRouter
- **Smart Responses** - Tailored responses with dog-like personality traits
- **Special Knowledge** - Includes fun easter eggs and crypto knowledge

### 🖥️ Desktop Features
- **Always on Top** - Optional overlay mode for constant availability
- **Roaming Mode** - Character can move around your screen automatically
- **System Tray Integration** - Minimize to system tray for background operation
- **Cross-Platform** - Works on Windows, macOS, and Linux

---

## 🚀 Installation

### Prerequisites
- **Node.js** (v16 or higher)
- **npm** or **yarn**
- **Git** (for cloning the repository)

### Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/Gerrald-sys/vrm-desktop-assistant.git
   cd vrm-desktop-assistant
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the application**
   ```bash
   npm start
   ```

### Building for Production

```bash
# Build for current platform
npm run build

# Build for specific platforms
npm run build-mac    # macOS
npm run build-win    # Windows
npm run build-linux  # Linux
```

---

## 🎮 Usage

### First Launch
1. **Start the application** using `npm start`
2. **Click the settings icon** ⚙️ to configure your API key
3. **Choose your AI provider** (OpenAI or OpenRouter)
4. **Enter your API key** from your chosen provider
5. **Click on the character** to start chatting!

### Interaction Guide

| Action | Description |
|--------|-------------|
| **Click Character** | Open chat interface |
| **Type & Enter** | Send message to AI |
| **Settings Button** | Open configuration panel |
| **System Tray** | Right-click for options menu |
| **Drag Character** | Move character around screen |

### Keyboard Shortcuts
- **Enter** - Send message
- **Shift + Enter** - New line in chat
- **Escape** - Close chat (when in settings)

---

## ⚙️ Configuration

### API Setup

#### OpenAI Setup
1. Visit [OpenAI Platform](https://platform.openai.com/api-keys)
2. Create a new API key
3. Copy the key (starts with `sk-`)
4. Paste in settings → OpenAI API Key

#### OpenRouter Setup  
1. Visit [OpenRouter](https://openrouter.ai/keys)
2. Create account and generate API key
3. Copy the key (starts with `sk-or-`)
4. Paste in settings → OpenRouter API Key

### Appearance Settings
- **Always on Top** - Keep character above other windows
- **Transparency** - Adjust character opacity (30-100%)
- **Chat Position** - Choose where chat appears (right/left/top/bottom)

### Advanced Settings
- **Roaming Mode** - Enable automatic character movement
- **Roaming Speed** - Control movement speed (1-10)
- **Auto-Hide Chat** - Automatically minimize chat after inactivity

---

## 🛠️ Development

### Project Structure
```
vrm-desktop-assistant/
├── src/
│   ├── main/           # Electron main process
│   │   ├── main.js     # Main application logic
│   │   └── preload.js  # Preload script for security
│   └── renderer/       # Frontend application
│       ├── index.html  # Main HTML structure
│       ├── app.js      # Application initialization
│       ├── vrm-renderer.js  # VRM model rendering
│       ├── chat-manager.js  # AI chat functionality
│       ├── settings.html    # Settings interface
│       └── styles.css  # Application styling
├── assets/             # Static assets
│   ├── dog.vrm        # Default VRM character model
│   ├── *.js           # Three.js and VRM libraries
│   └── *.png          # Icons and images
├── package.json       # Dependencies and scripts
└── README.md         # This file
```

### Technology Stack
- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **3D Rendering**: Three.js, VRM library
- **Desktop Framework**: Electron
- **AI Integration**: OpenAI API, OpenRouter API
- **Build Tools**: electron-builder

### Development Commands
```bash
npm start          # Start development server
npm run dev        # Start with auto-reload
npm run build      # Build for production
npm test           # Run tests (if available)
npm run lint       # Run code linting
```

### Contributing
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📋 Requirements

### System Requirements
- **OS**: Windows 10+, macOS 10.14+, Ubuntu 18.04+
- **RAM**: 512MB minimum, 1GB recommended
- **Storage**: 200MB for application
- **Graphics**: OpenGL 2.0 support for 3D rendering

### API Requirements
- **OpenAI API Key** OR **OpenRouter API Key**
- **Internet Connection** for AI functionality
- **Valid API credits** for AI conversations

---

## 🐛 Troubleshooting

### Common Issues

#### Character not loading
- Ensure VRM file is present in `assets/` folder
- Check console for Three.js errors
- Verify GPU acceleration is enabled

#### AI not responding
- Verify API key is correctly entered
- Check internet connection
- Ensure API provider has available credits
- Review console for API errors

#### Application crashes
- Update to latest Node.js version
- Clear application cache
- Reinstall dependencies with `npm ci`

#### Performance issues
- Reduce transparency settings
- Disable roaming mode
- Close other GPU-intensive applications

---

## 📝 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **VRM Consortium** - For the VRM character format
- **Three.js Team** - For the amazing 3D library
- **Electron Team** - For the cross-platform framework
- **OpenAI & OpenRouter** - For AI API services
- **Community Contributors** - For bug reports and feature suggestions

---

<div align="center">

**⭐ Star this repository if you find it helpful!**

Made with ❤️ and 🐕 by the VRM Desktop Assistant Team

[Report Bug](https://github.com/your-username/vrm-desktop-assistant/issues) • [Request Feature](https://github.com/your-username/vrm-desktop-assistant/issues) • [Documentation](https://github.com/your-username/vrm-desktop-assistant/wiki)

</div>
