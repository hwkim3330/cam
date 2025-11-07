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
- **P2P Mode**: Internet streaming with STUN servers
- **Auto NAT Traversal**: Works behind routers and firewalls
- **Automatic Quality**: Best resolution and bitrate selected automatically

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
3. Click "Start Webcam"
4. Share your ID or QR code with viewers
5. Done! Stream starts when viewer connects

### Viewer (Watching)
1. Open https://hwkim3330.github.io/cam/
2. Select **Watch** mode
3. Enter the broadcaster's ID
4. Click "Connect"
5. Start watching!

**Or** scan the QR code with your smartphone to auto-connect.

## 🛠️ Technical Details

### Technology Stack
- **WebRTC**: Peer-to-peer real-time communication
- **PeerJS**: Simple WebRTC abstraction library
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

## 🔧 Tips

### Network Optimization
- Use wired Ethernet for best quality
- Ensure good upload speed on broadcaster side
- Close bandwidth-heavy applications
- Check firewall allows UDP connections

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
- Verify webcam is not in use
- Try different browser
- Check console (F12) for errors

### High Latency
- Check network bandwidth
- Close bandwidth-heavy apps
- Use wired connection

### Connection Failed
- Verify correct ID entered
- Check both sides have internet
- Try refreshing the page
- Check firewall allows WebRTC

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
