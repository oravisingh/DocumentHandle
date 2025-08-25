PDF & Image Utility Toolkit

This is a browser-based utility project for performing common PDF and image tasks. It includes the following tools:

✅ Image Size Reducer (JPG, PNG to target size)

✅ JPG to PDF Converter

✅ PDF to JPG Converter

✅ PDF Merger

✅ PDF Splitter

✅ PDF to DOCX Converter



---

🧩 Project Structure

resourcePP/
├── assets/              # Logos, wallpapers, branding
├── backend/             # Python Flask backend APIs
├── frontend/            # HTML, CSS, JS frontend
├── static/              # Used by backend to store temporary files
└── test_resource/       # Your test files (not required for deployment)


---

⚙ Technologies Used

HTML, CSS, JavaScript (Vanilla)

Python 3

Flask (as backend API)

Ghostscript (for PDF compression)

Pillow (for image compression)



---

⚡ How to Run (Development Mode)

1. Install Python packages

pip install -r requirements.txt

2. Install Ghostscript

Make sure Ghostscript is installed and gswin64c or gs is available in the system path.

Download: https://www.ghostscript.com/download/gsdnld.html


3. Run Flask server

python backend/server.py

4. Open Frontend

Open frontend/index.html in your browser.

> Note: Tools like PDF compressor or PDF to DOCX will make requests to http://127.0.0.1:5000.




---

🚀 How to Run (Production Server)

If deploying on a university server or production:

1. Install Waitress (recommended for Windows)

pip install waitress

2. Run backend via Waitress

python backend/server.py

This will run the app on port 5000. You can reverse-proxy it through Nginx if needed.


---

📦 requirements.txt

Flask
flask-cors
Pillow
waitress


---

🔒 Security & Cleanup

All uploaded and generated files are stored in static/ and auto-deleted after use.

Files are served as downloads and not stored permanently.



---

👨‍🏫 Notes for University Deployment

This project is designed to be run locally or via a backend server like Waitress.

Please contact the technical cell if a reverse proxy or central deployment is required.

Frontend can be hosted as static files, the only requirement is that it should reach the backend server (localhost or remote).



---

🧠 Developed by

Ravinandan Samrat (B.Tech CSE, 3rd Year)

Contact: ornsamrat2004@gmail.com
