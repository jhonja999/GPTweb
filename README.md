# Local ChatGPT with Glassmorphic UI 🌠

A beautiful, private, and completely browser-based ChatGPT-like experience featuring a modern glassmorphic design and animated backgrounds. This implementation runs 100% locally in your browser, ensuring your conversations remain private and secure.

![image](https://github.com/user-attachments/assets/a4bbd0fd-c89e-4a8c-9c64-af87c5835988)

## ✨ Features

- **100% Local Processing**: All chat processing happens directly in your browser
- **Complete Privacy**: No data sent to external servers
- **Modern UI Design**:
  - Glassmorphic interface with blur effects
  - Animated meteor background
  - Smooth transitions and animations
  - Responsive design for all devices
- **Real-time Chat**:
  - Instant message updates
  - Typing indicators
  - Message history
- **Optimized Performance**:
  - Efficient worker-based processing
  - Smooth animations
  - Minimal resource usage

## 🚀 Getting Started

### Prerequisites

- Modern web browser (Chrome, Firefox, Safari, or Edge)
- Local development server

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/local-chatgpt-glass
cd local-chatgpt-glass
```

2. Start a local development server. You can use any of these methods:

Using Python:
```bash
python -m http.server 8000
```

Using Node.js (with `http-server`):
```bash
npx http-server
```

3. Open your browser and navigate to:
- Python: `http://localhost:8000`
- Node.js: `http://localhost:8080`

## 🛠️ Project Structure

```
local-chatgpt-glass/
├── index.html        # Main application file with UI
├── worker.js         # Web Worker for chat processing
└── README.md         # Documentation
```

## 💻 Usage

1. Open the application in your browser
2. Wait for the model to load (this may take a few moments)
3. Start chatting with the AI in the input field
4. Messages will appear in the chat window with smooth animations

## ⚙️ Technical Details

- Built with vanilla JavaScript and CSS
- Uses the MLC-AI/web-llm library for local processing
- Implements Web Workers for background processing
- CSS animations and transitions for smooth UI
- Glassmorphism effects using modern CSS features

### Model Information

The application uses the Llama-3-8B-Instruct model, which:
- Runs completely in the browser
- Requires no external API calls
- Provides fast response times
- Maintains privacy by processing all data locally

## 🎨 Customization

### Changing Colors

The UI uses CSS variables for easy customization. Edit the `:root` section in the CSS:

```css
:root {
  --glass-bg: rgba(255, 255, 255, 0.1);
  --glass-border: rgba(255, 255, 255, 0.2);
  --glass-shadow: rgba(0, 0, 0, 0.1);
}
```

### Modifying Animations

You can adjust meteor animation timing by modifying the interval in the JavaScript:

```javascript
setInterval(createMeteor, 2000); // Change 2000 to your preferred interval
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [MLC-AI/web-llm](https://github.com/mlc-ai/web-llm) for the local AI processing capability
- Inspired by modern glassmorphic UI design trends
- Built with love for the open-source community

## ⚠️ Important Notes

- First load may take some time as the model is downloaded
- Performance depends on your device's capabilities
- Requires a modern browser with WebAssembly support

## 📬 Contact

For questions and support, please open an issue in the GitHub repository.
