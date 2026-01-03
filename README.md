# Traffic-speed-Detection

# 🚦 Traffic Speed Detection using Computer Vision

This project uses computer vision techniques to detect and estimate the speed of vehicles in a video stream. It's built using Python, OpenCV, and NumPy. The goal is to help automate traffic analysis, potentially contributing to smart traffic systems and road safety monitoring.

## 📸 Demo
vehicles-result(3).mp4


## 🔧 Features

- ✅ Detects moving vehicles from a static camera
- 🎯 Calculates and displays vehicle speed in real-time
- 📐 Region of Interest (ROI) defined via perspective transformation
- 💾 Frame-by-frame analysis using OpenCV
- 📈 Logs detection info (e.g., frame, speed, time)

## 🛠️ Technologies Used

- Python 🐍
- OpenCV 📷
- NumPy 🔢
-Supervision
-Ulralytics

Make sure to place your video file in the correct folder and update the path inside .

## 🧠 How it Works

1. The video is read frame-by-frame.
2. A specific region of interest (ROI) is selected using a perspective transformation.
3. Background subtraction is used to detect motion.
4. Detected vehicle positions are tracked across frames.
5. Speed is estimated based on pixel distance and known physical conversion scale.

## 📏 Speed Estimation Formula

Speed is calculated using:


speed = distance / time


Converted to real-world units using a manually calibrated pixel-to-meter ratio.

## ⚠️ Limitations

- Works best with a fixed camera and clear lane visibility.
- Requires proper ROI setup for accurate results.
- Speed calibration depends on accurate pixel-to-meter ratio.

## 📌 To-Do

- [ ] Add multi-lane support
- [ ] Export speed logs to CSV
- [ ] Integrate object tracking (e.g., Deep SORT or ByteTrack)
- [ ] Live camera feed support

## 👨‍💻 Author

**Gershon Ayieko**  
📧 gershonayieko3@gmail.com  
📍 Nairobi, Kenya  
💼 [LinkedIn](https://linkedin.com) | 🐙 [GitHub](https://github.com/AyiekoGershon)

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

