# 📹 WebRTC Webcam Streaming

Ultra-low latency P2P video streaming solution using WebRTC technology. Stream your webcam with sub-200ms latency over local networks or the internet.

## 🌐 Live Demo

**https://hwkim3330.github.io/cam/**

## ✨ Features

### 🎥 Video Streaming
- **Ultra Low Latency**: Sub-200ms latency with P2P WebRTC
- **High Resolution**: Support from SD (640x480) to 4K (3840x2160)
- **Adaptive Quality**: Automatic bitrate adjustment based on network conditions
- **Multi-codec Support**: VP8, VP9, H.264 hardware acceleration

### 🌐 Network Modes
- **P2P Mode**: Internet streaming with STUN/TURN servers
- **LAN-Only Mode**: Direct local network connection (like GStreamer)
- **Auto NAT Traversal**: Works behind routers and firewalls

### 📊 Real-time Analytics
- **Resolution & Frame Rate**: Live video quality metrics
- **Bitrate Monitoring**: Upload/download bandwidth usage
- **Latency Tracking**: Round-trip time (RTT) measurement
- **Jitter Analysis**: Network stability indicators
- **Packet Loss Rate**: Connection quality assessment
- **Network Information**: IP addresses, transport protocol (UDP/TCP), connection type

### 📱 QR Code Sharing
- **Instant Connect**: Generate QR code for mobile viewers
- **Auto-connect**: Scan and start watching immediately
- **URL Sharing**: Share via messaging apps

### 📈 Performance Graphs
- **Real-time Charts**: Live visualization of metrics
- **30-second History**: Trend analysis
- **Multi-metric Display**: FPS, bitrate, latency, packet loss

## 🚀 Quick Start

### Broadcaster (Webcam Owner)
1. Open https://hwkim3330.github.io/cam/
2. Select **Broadcast** mode
3. Choose resolution (recommended: Full HD 1920x1080)
4. Select connection mode:
   - **P2P**: For internet streaming
   - **LAN Only**: For local network only
5. Click "Start Webcam"
6. Share the generated ID or QR code with viewers

### Viewer (Watching)
1. Open https://hwkim3330.github.io/cam/
2. Select **Watch** mode
3. Enter the broadcaster's ID
4. Click "Connect"
5. Start watching the live stream!

**Or** scan the QR code with your smartphone to auto-connect.

## 🛠️ Technical Details

### Technology Stack
- **WebRTC**: Peer-to-peer real-time communication
- **PeerJS**: WebRTC abstraction library
- **Chart.js**: Real-time performance charts
- **QRCode.js**: QR code generation
- **Vanilla JavaScript**: No framework dependencies

### Network Architecture
```
Broadcaster                    Viewer
    |                            |
    |------ WebRTC P2P --------->|
    |    (STUN/TURN assist)      |
    |                            |
    |<----- Stats Reports -------|
```

### LAN-Only Mode
When **LAN Only** is selected:
- No STUN/TURN servers used
- Direct peer-to-peer connection
- Minimal latency (50-100ms)
- Works only within same local network
- Perfect for:
  - Home surveillance
  - Local presentations
  - Internal testing
  - High-security environments

### Supported Browsers
- ✅ Chrome/Edge 80+
- ✅ Firefox 75+
- ✅ Safari 14+
- ✅ Opera 67+
- ✅ Mobile browsers (iOS Safari, Chrome Android)

## 📊 Performance Metrics

| Metric | Description | Typical Value |
|--------|-------------|---------------|
| **Latency** | Round-trip time | 50-200ms (LAN), 100-500ms (Internet) |
| **Bitrate** | Video data rate | 1-10 Mbps (depends on resolution) |
| **Frame Rate** | Frames per second | 30 fps |
| **Packet Loss** | Lost packets | <1% (good connection) |
| **Jitter** | Timing variation | <10ms (stable connection) |

## 🔧 Advanced Usage

### Custom Resolution
Edit the resolution dropdown to add custom sizes:
```html
<option value="3840x2160">4K - 3840x2160</option>
<option value="7680x4320">8K - 7680x4320</option>
```

### Network Optimization
For best performance:
- **LAN**: Use LAN-only mode, wired Ethernet preferred
- **Internet**: Use P2P mode, upload speed ≥ bitrate required
- **Low Bandwidth**: Choose lower resolution (HD or SD)
- **High Quality**: Choose Full HD or 4K with good network

### Firewall Configuration
If connection fails:
1. Ensure UDP ports are open
2. Check if STUN servers are accessible
3. Consider using LAN-only mode for local networks

## 🔒 Privacy & Security

- **No Server Storage**: All streaming is peer-to-peer
- **Temporary IDs**: Connection IDs change on each session
- **HTTPS Only**: Encrypted signaling
- **Local First**: LAN mode stays within your network
- **No Account Required**: Anonymous usage

## 🌟 Use Cases

### Professional
- 🎬 Live presentations and demos
- 📡 Remote monitoring and surveillance
- 🎓 Online teaching and tutoring
- 👥 Video conferencing (1-to-1)

### Personal
- 🏠 Home security camera
- 👶 Baby monitor
- 🐾 Pet cam
- 🎮 Gameplay streaming (webcam)

### Development
- 🧪 WebRTC testing
- 📊 Network analysis
- 🔬 Latency research
- 💻 Video codec comparison

## 🐛 Troubleshooting

### No Video Showing
- Check browser permissions (camera/microphone)
- Verify webcam is not used by another application
- Try different browser
- Check F12 console for errors

### High Latency
- Switch to LAN-only mode if on same network
- Check network bandwidth
- Reduce resolution
- Close bandwidth-heavy applications

### Connection Failed
- Verify both sides have internet access (P2P mode)
- Check firewall settings
- Try LAN-only mode for local networks
- Ensure correct ID is entered

## 📝 License

MIT License - feel free to use for personal or commercial projects

## 🤝 Contributing

Contributions are welcome! Please feel free to submit pull requests.

## 📬 Support

For issues or questions:
- Open an issue on GitHub
- Check browser console for error messages
- Verify WebRTC is supported in your browser

---

**Built with ❤️ using WebRTC**

*Zero server costs, infinite possibilities*
