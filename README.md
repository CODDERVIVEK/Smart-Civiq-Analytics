# 🏛️ Smart Civic Analytics

**ML-powered queue management system for government offices — predicts wait times, issues virtual tokens, and notifies citizens via SMS.**

click on Demo....

## What It Does

Smart Civic Analytics brings order to government office queues. Citizens get a virtual token, see their real-time wait, and receive an SMS when it's their turn — all driven by machine learning models.

- 🤖 **Predicts wait times** using XGBoost & Random Forest
- 🎫 **Issues virtual tokens** with unique IDs and queue position
- 📲 **Sends SMS alerts** via Twilio when token is called
- 🔁 **Recovers missed tokens** with smart slot re-insertion
- 📊 **Forecasts crowd levels** up to 2 hours ahead
- 👴 **Prioritizes senior citizens** (age 70+) automatically

---

## Live Demo

🚀 [smart-civiq-analytics.streamlit.app](https://smart-civiq-analytics-hruhonyqqvcjt99dft9nde.streamlit.app/)

---

## Tech Stack

| | |
|---|---|
| **UI** | Streamlit |
| **ML Models** | XGBoost, Random Forest |
| **SMS** | Twilio |
| **Data** | Pandas, NumPy |
| **Deployment** | Streamlit Cloud |

---

## Quick Start

```bash
cd Smart-Civiq-Analytics
pip install -r requirements.txt
```

Create a `.env` file:
```
TWILIO_ACCOUNT_SID=your_sid
TWILIO_AUTH_TOKEN=your_token
TWILIO_PHONE_NUMBER=+91XXXXXXXXXX
```

Train models and run:
```bash
python train_models.py
streamlit run dashboard.py
```

---

## ML Models

Two models trained on civic queue data:

- **XGBoost** — predicts wait time in minutes
- **Random Forest** — forecasts queue size +1hr and +2hr ahead

Input features: place, day, hour, queue length, counters open, service time, weather, holiday flag.

---

## Built By

**Vivek Gaikwad**
---

*If this helped you, drop a ⭐ on GitHub!*
