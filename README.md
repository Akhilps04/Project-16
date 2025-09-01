## Satellite Pass Notification and Data Availability System

🚀 **Global Nominee – NASA Space Apps Challenge 2024**

This project was developed as part of the **NASA Space Apps Challenge 2024**, where it was selected as a **Global Nominee finalist**. It is a Flask-based web application that allows users to:

* Get upcoming **satellite pass predictions** (with a focus on Landsat 8 and Landsat 9).
* Receive **email notifications** before a satellite pass.
* Estimate **data availability times** after the pass.
* Visualize a **3x3 Landsat pixel grid** around a given location using Folium maps.
* Optionally integrate with **Google Earth Engine** for further analysis.

---

## 📂 Folder Structure

```
main/
│── app/                # Core Flask application code
│── data/               # Skyfield TLE data cache
│── env/                # Environment variables (.env file goes here)
│── static/             # Static files (maps, CSS, JS, etc.)
│── templates/          # HTML templates for rendering pages
│── README.md           # Project documentation
```

---

## ⚙️ Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/your-username/your-repo.git
cd main
```

### 2. Create and activate a virtual environment

```bash
python3 -m venv venv
source venv/bin/activate   # On Linux/Mac
venv\Scripts\activate      # On Windows
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure environment variables

Create a `.env` file inside the `env/` folder with the following:

```
SENDER_EMAIL=your_email@gmail.com
SENDER_PASSWORD=your_app_password
```

⚠️ Use an **App Password** if you are using Gmail.

### 5. Run the Flask app

```bash
python app/app.py
```

The app will be available at:
👉 `http://127.0.0.1:5000/`

---

## 📡 Features

* **Satellite Pass Prediction**: Uses Skyfield and Celestrak TLEs to compute passes.
* **Email Notifications**: Sends reminders before satellite passes using Gmail SMTP.
* **Data Availability Estimation**: Predicts when Landsat data may be available (6 hours after pass).
* **Map Visualization**: Displays a 3x3 Landsat pixel grid centered on user location with Folium.
* **Earth Engine Integration**: Ready for connecting with Google Earth Engine for advanced analysis.

---

## 🛰️ Tech Stack

* **Backend**: Flask (Python)
* **Scheduler**: APScheduler
* **Satellite Data**: Skyfield, Celestrak TLEs
* **Mapping**: Folium, Leaflet
* **Email Service**: SMTP (Gmail)
* **Optional**: Google Earth Engine

---

## 🏆 Recognition

This project was selected as a **Global Nominee finalist** in the **NASA Space Apps Challenge 2024**, representing innovative use of open space and Earth data to solve real-world problems.

---
## Acknowledgments

Thanks to my mentors and colleagues for their guidance.

---

## 📜 License

This project is for academic and demonstration purposes only. Please credit the authors if reused or modified.

---
