# ⚡ Energy Consumption & Power Demand Prediction
### AI-Driven Forecasting Using Deep Learning & Real-Time Weather Inputs

This project is a **Flask-based web application** that predicts the **next-step power demand** using historical energy consumption (5-minute interval data) combined with **weather conditions**.  
It features an interactive UI, analytics, energy guidance, and awareness resources — making it valuable for:

- Power grid operations  
- Industry energy management  
- Smart city platforms  
- Academic & research applications  

---

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

