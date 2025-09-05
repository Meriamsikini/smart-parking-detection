# 🚗 Smart Parking Detection

## 📌 Project Description
**Smart Parking Detection** is a computer vision project that automatically detects available and occupied parking spaces from a surveillance video.  
It combines **image classification** with a **machine learning model** and **real-time video processing** to provide accurate parking occupancy detection.  

This project is designed as a proof of concept for **smart cities** and **IoT-based parking management systems**.  

---

## 🔹 Features
- Automatic detection of parking slots using a predefined mask.
- Image classification (`empty` vs `not_empty`) with a trained ML model.
- Change-detection optimization: only reclassifies slots when significant differences occur between frames.
- Real-time visualization with bounding boxes:  
  - 🟩 Green = Available  
  - 🟥 Red = Occupied
- Counter displaying the number of free slots vs total slots.
- Saves an annotated video with all results.

---

## 🔹 Tech Stack
- **Python 3.x**
- **OpenCV** → image & video processing
- **scikit-learn** → machine learning & PCA
- **scikit-image** → image preprocessing
- **NumPy / Matplotlib** → data manipulation & visualization

---

## 📂 Project Structure
## 📂 Project Structure
`data/ (clf-data.zip, parking_1920_1080.mp4, mask_crop.png, mask_1920_1080.png), model/ (model.pkl), src/ (data_preparation.ipynb, main.py, utils.py), output/, requirements.txt, README.md`



---

## 🖼 Screenshot
![Parking Detection Screenshot](https://your-image-link-here.com/screenshot.png)  


---

## ⚙️ Installation
1. Clone the repository:
```bash
git clone https://github.com/Meriamsikini/smart-parking-detection.git
cd smart-parking-detection

Install dependencies:

``` bash

pip install -r requirements.txt
```
## ▶️ Usage
Make sure your dataset, video, and mask are placed inside the data/ directory.

Run the main script:

```bash
python src/main.py
```
✅ The video will open in a window showing green and red bounding boxes with the number of available slots.

✅ An annotated video will also be saved inside the output/ directory.

## 📊 Results
Real-time visualization of parking occupancy.

Annotated video showing detected slots as free or occupied.

PCA projection (from data_preparation.ipynb) for understanding dataset separation.

## 🚀 Use Cases
Smart city intelligent parking systems.

Real-time parking lot monitoring.

Integration with IoT sensors and dashboards.

## 👩‍💻 Author
Meriam Sikini
