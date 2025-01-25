# 🏦 Parking Space Counter Project

This project leverages Python and OpenCV to detect parking space availability in video footage. It consists of two main scripts:

1. **main.py**: Detects and displays parking space availability in a parking lot video.
2. **parkingspacepicker.py**: Allows the user to interactively mark and remove parking spaces on a reference image.

---

## ✨ Features

- 🎥 Detect available and occupied parking spaces from a video feed.
- ✍️ Interactive tool to define or update parking space positions.

---

## 🔧 How to Use

### Step 1: Define Parking Spaces

1. Run the `parkingspacepicker.py` script:
   ```bash
   python parkingspacepicker.py
   ```

2. Use the following mouse actions on the `carParkImg.png` image:
   - **⬅ Left Click**: Add a parking space.
   - **➡ Right Click**: Remove a parking space.

3. Positions will be saved automatically to a file named `CarParkPos`.

---

### Step 2: Detect Parking Space Availability

1. Place your parking lot video as `carPark.mp4` in the root directory.
2. Run the `main.py` script:
   ```bash
   python main.py
   ```
3. The script processes the video and displays:
   - 🔹 Parking space status (Free/Occupied).
   - 🔹 Count of available and total spaces in real time.

---

## 📁 File Descriptions

### main.py

- Reads a parking lot video (`carPark.mp4`).
- Processes the video frame-by-frame using OpenCV for parking space detection.
- Displays parking space status on the video feed in real time.

### parkingspacepicker.py

- Reads a reference image of the parking lot (`carParkImg.png`).
- Enables interactive selection and removal of parking spaces using the mouse.
- Saves marked positions to a file (`CarParkPos`) using the `pickle` module.

---

## 🔗 Prerequisites

- Python 3.x
- Required Python libraries:
  - OpenCV
  - NumPy
  - cvzone

Install these libraries using pip:
```bash
pip install opencv-python-headless numpy cvzone
```

---

## 🚧 Note

Ensure the following files are placed in the root directory before running the scripts:
- `carParkImg.png` (Reference image for marking parking spaces).
- `carPark.mp4` (Video file of the parking lot).

---

## 🎨 Example Outputs

- **parkingspacepicker.py**:
  - Interactive image with parking spaces marked as rectangles.

- **main.py**:
  - Video with live updates on parking space availability, marked in 🟢 green (Free) or 🔴 red (Occupied).

---

Feel free to ✨ fork and modify this project according to your needs. Happy coding! 🚀

