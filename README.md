# 📹 Cam - Computer Vision & WebRTC Demos

Collection of real-time computer vision, AI, and video streaming demos using webcam.

## 🎯 Live Demos

### 🏋️ AI Fitness Trainer (NEW!)
**Your personal AI-powered workout assistant**

🔗 **[Try AI Fitness Trainer](https://hwkim3330.github.io/cam/fitness-trainer.html)**

**Features:**
- 🏋️ **4 Exercises**: Squat, Push-Up, Jumping Jack, Plank
- 🤖 **AI Rep Counting**: Automatic detection and counting
- 📐 **Angle Detection**: Validates proper form using joint angles
- 💬 **Real-time Feedback**: "Perfect form!" or "Keep body straight"
- 🔥 **Calorie Tracking**: Estimates calories burned
- ⏱️ **Workout Timer**: Tracks exercise duration
- 📊 **Progress Charts**: Visualize your improvement (Chart.js)
- 💾 **Workout History**: Saves last 50 workouts
- 🎯 **Daily Goals**: Track progress toward 50 reps/day
- 🎨 **Apple Fitness+ UI**: Beautiful gradient purple design

**How it Works:**
1. Select exercise (Squat, Push-up, Jumping Jack, or Plank)
2. Click "Start" and begin exercising
3. AI detects your pose and counts reps automatically
4. Get real-time feedback on your form
5. View stats and history in side panel

**Exercise Detection:**
- **Squat**: Knee angle detection (< 100° down, > 160° up)
- **Push-Up**: Elbow angle detection (< 90° down, > 160° up)
- **Jumping Jack**: Arms + legs position tracking
- **Plank**: Body alignment validation (160-200°)

---

### 🦴 Pose Analytics V2
**Real-time multi-person pose tracking with depth awareness**

🔗 **[Try Pose Analytics V2](https://hwkim3330.github.io/cam/pose-analytics-v2.html)**

**Features:**
- 🦴 Real-time skeleton tracking (MoveNet MultiPose - up to 10 people)
- 👤 Face detection with age/gender estimation
- 📏 Height estimation with depth awareness
- 📍 Distance from camera calculation
- 🎨 **Adjustable skeleton rendering (Settings tab)**
  - Line Width: 4-16px
  - Keypoint Size: 4-20px
  - Glow Intensity: 0-30
  - Detection Sensitivity: 0.1-0.5
- 🏃 Activity recognition (Standing, Sitting, Walking, Raising Hand)
- 💾 Export all data as JSON
- 📋 Real-time event logging

**Calibration:**
- Default calibration included (works immediately)
- Optional custom calibration in Settings tab
- Depth-aware measurements using shoulder width

**Troubleshooting:**
- If skeleton not visible → Go to ⚙️ Settings tab
- Increase Line Width to 16px
- Increase Glow Intensity to 30
- Increase Keypoint Size to 20px

---

### 🦴 Pose Analytics V1
**Original pose tracking with enhanced visualizations**

🔗 **[Try Pose Analytics V1](https://hwkim3330.github.io/cam/pose-analytics.html)**

Features:
- Multi-person pose detection
- Age & gender estimation
- Height prediction
- Activity tracking
- Real-time FPS counter
- Enhanced skeleton rendering with glow effects

---

### 🧩 Hand Gesture Puzzle CAPTCHA
**Apple-style puzzle verification with hand gestures**

🔗 **[Try Puzzle CAPTCHA](https://hwkim3330.github.io/cam/puzzle-captcha.html)**

**Features:**
- MediaPipe hand tracking
- 4x4 webcam puzzle grid
- 🤏 Pinch gesture to grab & move pieces
- 📱 Touch support for mobile devices
- ✨ Smooth animations
- ✓ Verification on completion

**How to Play:**
1. Pinch thumb + index finger together
2. Move hand to drag puzzle piece
3. Release to drop
4. Arrange all 16 pieces correctly

---

### 📹 WebRTC Ultra Low-Latency Streaming
**P2P video streaming with sub-200ms latency**

🔗 **[Try WebRTC Stream](https://hwkim3330.github.io/cam/index.html)**

**Features:**
- **Ultra Low Latency**: Sub-200ms P2P streaming
- **High Resolution**: SD to 4K support
- **Real-time Analytics**: FPS, bitrate, latency, packet loss
- **QR Code Sharing**: Instant mobile connection
- **Performance Graphs**: 30-second history charts

**Usage:**
- **Broadcaster**: Start webcam → Share ID/QR
- **Viewer**: Enter ID → Connect → Watch

---

## 🚀 Quick Start

### For Pose Analytics V2:
1. Open the demo link
2. Allow camera access
3. See yourself with skeleton overlay
4. Adjust rendering in **⚙️ Settings tab** if needed

### For Puzzle CAPTCHA:
1. Open demo
2. Allow camera
3. Pinch with fingers to grab pieces
4. Solve the puzzle!

### For WebRTC Streaming:
1. **Broadcaster**: Start webcam → Share ID
2. **Viewer**: Enter ID → Connect
3. Ultra-low latency streaming starts!

---

## 🛠️ Technologies

### AI & Computer Vision
- **TensorFlow.js** - Browser-based machine learning
- **MoveNet MultiPose Lightning** - Fast multi-person pose detection
- **MediaPipe** - Hand tracking & face detection
- **Canvas API** - Real-time rendering with effects

### Networking
- **WebRTC** - Peer-to-peer communication
- **PeerJS** - Simplified WebRTC
- **STUN/TURN** - NAT traversal

### UI/UX
- **Apple Design Language** - Clean, minimal interface
- **Chart.js** - Performance visualization
- **QRCode.js** - Mobile sharing
- **Vanilla JavaScript** - No framework bloat

---

## 📊 Performance

| Demo | FPS | Latency | Max People |
|------|-----|---------|------------|
| AI Fitness Trainer | 30-60 | <30ms | 1 |
| Pose Analytics V2 | 30-60 | <50ms | 10 |
| Pose Analytics V1 | 30-60 | <50ms | 10 |
| Puzzle CAPTCHA | 30-60 | <30ms | 1 |
| WebRTC Stream | 30 | 50-200ms | 2 |

**System Requirements:**
- Modern browser (Chrome/Edge recommended)
- Webcam
- GPU acceleration (optional but recommended)
- HTTPS connection (required for camera access)

---

## ⚙️ Settings & Customization

### Pose Analytics V2 Settings

**Display Options:**
- `Skeleton Line Width`: 4-16px (default: 10px)
- `Keypoint Size`: 4-20px (default: 12px)
- `Glow Intensity`: 0-30 (default: 15)

**Detection:**
- `Min Confidence`: 0.1-0.5 (default: 0.2)
  - Lower = more detections
  - Higher = more accurate

**Calibration:**
- Default: 170cm reference height
- Custom: Enter your height for accuracy

---

## 🔧 Troubleshooting

### Skeleton Not Visible?
**Solution:** Go to ⚙️ Settings tab and adjust:
1. Skeleton Line Width → **16px**
2. Glow Intensity → **30**
3. Keypoint Size → **20px**
4. Min Confidence → **0.15**

### Low FPS?
1. Close other tabs/applications
2. Enable hardware acceleration in browser
3. Use Chrome/Edge for best performance
4. Lower detection sensitivity in Settings

### Camera Not Working?
1. Check browser permissions (camera icon in URL bar)
2. Verify HTTPS connection
3. Try different browser
4. Refresh page and allow camera again

### Height Measurements Inaccurate?
1. Go to Settings → Height Calibration
2. Enter your real height
3. Stand at comfortable distance
4. Click "Calibrate Now"

---

## 🎨 Features by Demo

### Pose Analytics V2
✅ Multi-person tracking
✅ Depth-aware height estimation
✅ Distance measurement
✅ Adjustable rendering
✅ Activity recognition
✅ Age/gender estimation
✅ Data export
✅ Event logging

### Puzzle CAPTCHA
✅ Hand gesture control
✅ Touch support
✅ 4x4 puzzle grid
✅ Real-time webcam capture
✅ Verification system

### WebRTC Streaming
✅ P2P streaming
✅ Ultra-low latency
✅ QR code sharing
✅ Real-time analytics
✅ Multi-codec support

---

## 🔒 Privacy & Security

- **No Server Storage**: All processing in browser
- **No Data Transmission**: Computer vision runs locally
- **P2P Only**: WebRTC uses direct connections
- **Temporary Sessions**: No persistent data
- **No Account Required**: Anonymous usage
- **HTTPS**: Secure camera access

---

## 📝 Notes

- All demos run entirely in browser (no server required)
- AI models downloaded once and cached
- No data leaves your device (except WebRTC P2P)
- Works offline after first load (except WebRTC)
- Best performance on Chrome/Edge with GPU

---

## 🌟 Use Cases

### Professional
- 🎬 Pose analysis for fitness/sports
- 🏥 Remote health monitoring
- 🎓 Online teaching with activity tracking
- 🎨 Motion capture for animation

### Security
- 🔐 Gesture-based CAPTCHA
- 👤 Person counting and tracking
- 🚶 Activity monitoring

### Development
- 🧪 Computer vision testing
- 📊 Performance benchmarking
- 🔬 ML model experimentation

---

## 🔗 Links

- **GitHub Repository**: [hwkim3330/cam](https://github.com/hwkim3330/cam)
- **AI Fitness Trainer**: https://hwkim3330.github.io/cam/fitness-trainer.html
- **Pose Analytics V2**: https://hwkim3330.github.io/cam/pose-analytics-v2.html
- **Pose Analytics V1**: https://hwkim3330.github.io/cam/pose-analytics.html
- **Puzzle CAPTCHA**: https://hwkim3330.github.io/cam/puzzle-captcha.html
- **WebRTC Stream**: https://hwkim3330.github.io/cam/index.html

---

## 📬 Support

For issues:
1. Check browser console (F12) for errors
2. Try troubleshooting steps above
3. Open GitHub issue with details
4. Include: Browser version, OS, error message

---

**Made with Claude Code** 🤖
*Zero server costs, infinite possibilities*
