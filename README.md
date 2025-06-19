# Hero Video Background Player

A modern, responsive hero section with video background, featuring smooth animations, subtitle support, and adaptive playback controls.

## 🌟 Features

- **Video Background**: Supports WebM and MP4 formats with automatic fallback
- **Smart Playback**: Auto-pause when scrolling away, resume when returning
- **Subtitle Support**: WebVTT subtitle display with custom styling
- **Responsive Design**: Optimized for desktop and mobile devices
- **Elegant Controls**: Glassmorphism-styled play button with pulse animation
- **Progress Tracking**: Real-time video progress indicator
- **Fallback Support**: Graceful degradation to background images when video unavailable

## 🚀 Demo

![Hero Video Player Preview](preview.gif)

## 📁 Project Structure

```
project/
├── hero.html              # Main HTML file
├── resources/
│   ├── background.webm     # Primary video file (WebM format)
│   ├── background.mp4      # Fallback video file (MP4 format)
│   ├── background.png      # Background image fallback
│   ├── description.txt     # Title and description content
│   └── subtitles.vtt       # WebVTT subtitle file
└── README.md
```

## 📋 Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/hero-video-background.git
cd hero-video-background
```

### 2. Prepare Your Content Files

Create a `resources/` folder and add your content:

#### Video Files (choose one or both):
- `background.webm` - Primary video format (recommended for web)
- `background.mp4` - Fallback video format

#### Background Image:
- `background.png` - Static background image (shown when video ends or unavailable)

#### Text Content:
- `description.txt` - Text file where:
  - **First line**: Video title
  - **Remaining lines**: Video description

Example `description.txt`:
```
Amazing Product Launch
Discover our revolutionary new product that will change
how you think about technology. Join us on this incredible
journey of innovation and excellence.
```

#### Subtitles (optional):
- `subtitles.vtt` - WebVTT format subtitle file

Example `subtitles.vtt`:
```
WEBVTT

00:00.000 --> 00:03.000
Welcome to our amazing product

00:03.000 --> 00:06.000
Experience the future today
```

### 3. Launch the Application

Open `hero.html` in your web browser or serve it through a local web server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (http-server)
npx http-server

# Then visit: http://localhost:8000
```

## 🎨 Customization

### Styling
The player uses CSS custom properties for easy theming. Key elements you can customize:

- **Colors**: Modify gradient backgrounds and overlay colors
- **Typography**: Change fonts and text sizes in the CSS
- **Animations**: Adjust pulse animation timing and effects
- **Layout**: Modify positioning and spacing

### Video Settings
- **Autoplay**: Video starts muted and plays after user interaction
- **Loop**: Currently disabled - video ends and shows background image
- **Quality**: Supports any resolution, optimized for 1920x1080

### Responsive Breakpoints
- **Desktop**: Full feature set with large controls
- **Mobile** (768px and below): Optimized layout with smaller controls

## 🔧 Browser Support

- **Modern Browsers**: Chrome 80+, Firefox 75+, Safari 13+, Edge 80+
- **Video Formats**: WebM (preferred), MP4 (fallback)
- **Features Used**: 
  - CSS Grid & Flexbox
  - Intersection Observer API
  - ES6 Modules & Async/Await
  - WebVTT Subtitles

## 📱 Mobile Optimization

- Touch-friendly controls
- Reduced animation complexity
- Optimized text sizing
- Gesture-friendly interface
- Bandwidth-conscious loading

## 🎯 Use Cases

- **Landing Pages**: Product launches, marketing campaigns
- **Portfolio Sites**: Creative showcases, agency websites  
- **Corporate Sites**: Company introductions, brand stories
- **Event Pages**: Conference announcements, webinar promotions

## 🛠️ Technical Details

### Key Components:
- **HeroVideoPlayer Class**: Main JavaScript controller
- **Intersection Observer**: Handles scroll-based play/pause
- **Resource Loading**: Automatic file detection with fallbacks
- **WebVTT Parser**: Custom subtitle parsing and display
- **Progress Tracking**: Real-time playback progress

### Performance Features:
- Lazy loading of video resources
- Efficient DOM manipulation
- Optimized CSS animations
- Memory-conscious event handling

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Modern CSS techniques and animations
- WebVTT specification for subtitle support
- Intersection Observer API for scroll detection
- Glassmorphism design trends

## 📞 Support

If you encounter any issues or have questions:

1. Check the [Issues](https://github.com/yourusername/hero-video-background/issues) page
2. Create a new issue with detailed information
3. Include browser version and console errors if applicable

---

**Made with ❤️ for modern web experiences**
