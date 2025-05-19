# 🗜️ ZIPMAN - Huffman-Based File Compression Web App

**ZIPMAN** is an intuitive, browser-based file compressor and decompressor that uses **Huffman Encoding** to compress `.txt`, `.pdf`, and image files. It supports drag-and-drop functionality, live compression ratio display, and is built using Flask and JavaScript.

---

## 🚀 Features

- 📁 Upload and compress `.txt`, `.pdf`, and image files
- 📦 Huffman-based encoding for efficient text compression
- 🖼️ Drag-and-drop UI for text, image, and PDF handling
- 🔁 Decompression restores files to original form
- 📊 Displays real-time compression ratio
- 💬 Alerts for invalid file sizes or types
- 🎥 Animated backgrounds and stylized UI using Bootstrap 5

---

## 🛠️ Tech Stack

| Layer       | Technology       |
|-------------|------------------|
| Backend     | Python, Flask    |
| Frontend    | HTML, CSS, JS    |
| Compression | Huffman Coding   |
| UI Library  | Bootstrap 5      |
| Fonts       | Custom (.ttf)    |

---

## 📂 Project Structure

  <pre>zipman/ 
    ├── app.py                         # Main Flask application with Huffman compression logic 
    ├── info.txt                       # Font license and reference 
    ├── requirements.txt               # (Optional) Python dependencies file 
    
    ├── templates/                     # HTML templates for different pages 
    │ ├── index.html                   # Homepage (file compression UI) 
    │ ├── image.html                   # Image compression UI 
    │ ├── pdf.html                     # PDF compression UI 
   
    ├── static/                        # Static assets (fonts, videos, images) 
    │ └── public/ 
    │ ├── zipman_logo.jpg              # Logo image 
    │ ├── *.ttf                        # Custom fonts 
    │ ├── *.mp4                        # Background videos
   
    │ ├── nwcursor.png                 # Custom cursor (if used) 
    └── README.md                      # Project documentation (this file) </pre>
---

## 🧠 How It Works

### 🔹 Compression Flow
1. Files are read and merged (if multiple).
2. Character frequencies are computed.
3. Huffman Tree is built and encoded.
4. Data is compressed to a binary-like stream and returned.

### 🔹 Decompression Flow
1. Huffman Tree is reconstructed from metadata.
2. Encoded binary data is decoded.
3. Original file is restored and made downloadable.

---

## 🖥️ Running Locally

### 1. Clone the Repository
    git clone https://github.com/yourusername/zipman.git
    cd zipman
  
### 2.(Optional) Create a Virtual Environment
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate

### 3. Install Required Packages
    pip install Flask

### 4. Run the Flask App
    python app.py

#### Then, open your browser and visit:
    http://127.0.0.1:5000

---

## 📸 Screenshots
![Screenshot (30)](https://github.com/user-attachments/assets/6cfd2cfe-12ca-4e6f-8473-2bab97a3c071)
![Screenshot (31)](https://github.com/user-attachments/assets/7d777b32-8165-4d39-9b0b-f22e23e72c76)
