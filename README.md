# ⚡ Energy Consumption & Power Demand Prediction
### AI-Driven Forecasting Using Deep Learning & Real-Time Weather Inputs

This project is a **Flask-based web application** that predicts the **next-step power demand** using historical energy consumption (5-minute interval data) combined with **weather conditions**.  
It features an interactive UI, analytics, energy guidance, and awareness resources — making it valuable for:

- Power grid operations  
- Industry energy management  
- Smart city platforms  
- Academic & research applications  

---
## Website Link
https://web-production-bd8d.up.railway.app

## 🚀 Key Features

### 🔮 1. Next-Step Power Demand Prediction
Upload the last **30 rows** (each representing a 5-minute interval) of these features:

- Power demand  
- Temperature  
- Dew point  
- Humidity  
- Wind direction  
- Wind speed  
- Pressure  

The app processes this window and predicts the **next 5-minute energy demand**.

---

### 📊 2. Visualization
- Line charts showing:
  - Last 30 power demand values  
  - Predicted next point  
- Table displaying modified feature window

---

### 🧠 3. Deep Learning Model
- Framework: **TensorFlow/Keras**
- Input: **(30 timesteps × 7 features)**
- Scalers Used:
  - `scaler_features.pkl`
  - `scaler_target.pkl`
- Saved as: **`.h5` model format**

---

### 💡 4. Smart Energy Guidance (UI Demo)
Includes:
- Personalized savings layout  
- Appliance consumption breakdown  
- Off-peak usage recommendations  
- Seasonal optimization tips  

---

### 🌍 5. Awareness Page
Provides informative cards about:
- Renewable energy  
- Carbon footprint  
- Efficient appliances  
- Sustainable habits  

---

### 📑 6. About Page
Covers:
- Dataset description  
- Model architecture  
- Training workflow  
- Project motivation  
- Tech stack  

---

## 🗂️ Project Structure
├── app.py
├── power_model.h5
├── scaler_features.pkl
├── scaler_target.pkl
├── requirements.txt
├── Procfile
├── templates/
│ ├── base.html
│ ├── predict.html
│ ├── guidance.html
│ ├── awareness.html
│ ├── analysis.html
│ ├── about.html
├── static/
│ ├── css/
│ ├── js/
│ ├── assets/
├── README.md


---

## ⚙️ Tech Stack

### Frontend
- HTML5, CSS3, Bootstrap 5  
- Chart.js  

### Backend
- Python 3.11  
- Flask  
- Pandas, NumPy  
- TensorFlow/Keras  
- scikit-learn  

### Deployment
- Railway  
- Gunicorn  
- Works with Docker (optional)  

---

## 📥 How to Run Locally

### 1️⃣ Clone Repository
```bash
git clone https://github.com/your-username/energy-consumption.git
cd energy-consumption
pip install -r requirements.txt
python app.py
http://127.0.0.1:5000/
```
## 📊 Dataset Details

Dataset contains **5-minute interval energy consumption (2021–2024)** along with **weather features**.

### **Features Used**

| Feature        | Description                          |
|----------------|--------------------------------------|
| Power demand   | Historical consumption (target)      |
| Temperature    | Ambient temperature                  |
| Dew Point      | Atmospheric dew point                |
| Humidity       | Relative humidity (%)                |
| Wind Direction | Direction of wind                    |
| Wind Speed     | Speed of wind                        |
| Pressure       | Atmospheric pressure                 |

Weather features significantly influence energy load patterns, helping improve prediction accuracy.

---

## 🧠 Model Training Methodology

- Uses **30-step sliding window** for time-series forecasting  
- Features scaled using **MinMaxScaler**  
- Model Architecture: **Deep Learning Hybrid (LSTM + CNN blend)**  
- Optimizer: **Adam**  
- Loss Function: **Mean Squared Error (MSE)**  
- Output: **1 predicted value** → next 5-minute energy demand  

---

## 🌐 Deployment Notes

- `.keras` models may break in cloud environments  
- `.h5` format is **universally compatible** → recommended for production  
- Supported Deployment Platforms:  
  - **Railway**  
  - **Render**  
  - **Docker**  

---

## 🤝 Contributing

Contributions are welcome!  
Feel free to open an **Issue** or **Pull Request** to improve:
- UI/UX  
- Model performance  
- Dataset quality  
- Documentation  

---

## 📄 License

Released under the **MIT License**.

---

## ⭐ Support

If this project helped you, consider giving the repository a **🌟 star** — it really motivates future improvements!
