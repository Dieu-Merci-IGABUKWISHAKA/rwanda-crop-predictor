# Rwanda Crop Yield & Market Price Predictor 🌾

A full end-to-end machine learning web application that predicts:
- **Expected crop yield** (kg/ha)
- **Expected market price** (RWF/kg)

for Rwandan farmers and agriculture officers based on crop type,
district, season, and automatically fetched live weather data.

## Problem Statement
Farmers in Rwanda make planting and selling decisions without reliable
data on expected yields or market prices. This tool gives them
data-driven predictions so they can plan better and earn more.

## Who Uses This
| User | How they use it |
|---|---|
| Individual farmers | Know expected yield and best time to sell |
| Cooperatives | Plan collective planting and selling strategy |
| RAB / MINAGRI | National food security planning |
| NGOs / WFP | Early warning for food shortage prediction |

## How It Works
1. User selects crop type, district, and season on the web form
2. App automatically fetches live weather data (rainfall, temperature)
   from Open-Meteo API using the district coordinates
3. Two ML models run simultaneously
4. Results displayed instantly on screen

## Predictions
| Output | Unit | Model |
|---|---|---|
| Expected crop yield | kg/ha | yield_model.pkl |
| Expected market price | RWF/kg | price_model.pkl |

## Tech Stack
| Layer | Technology |
|---|---|
| Data storage | MySQL |
| Data processing | Python, Pandas, NumPy |
| Visualization | Matplotlib, Seaborn, Power BI |
| Machine learning | Scikit-learn |
| Backend | Django 5.2 |
| Frontend | HTML, CSS |
| Weather data | Open-Meteo API (free, no key needed) |
| Deployment | Render.com |

## Project Structure
```
rwanda-crop-predictor/
├── data/              # Raw datasets (not tracked by git)
├── notebooks/         # Jupyter EDA notebooks
├── ml_model/          # Trained model files (.pkl)
├── django_app/        # Django web application
├── requirements.txt   # All Python dependencies
└── README.md          # Project documentation
```

## Dataset Sources
- FAO FAOSTAT — crop yield data per country (free CSV download)
- World Bank Climate — rainfall and temperature data
- Kaggle — Africa crop market price datasets
- Open-Meteo API — live weather by coordinates (no signup needed)

## Project Phases
- [ ] Phase 1 — Data collection
- [ ] Phase 2 — Data cleaning
- [ ] Phase 3 — Exploratory data analysis
- [ ] Phase 4 — ML model training
- [ ] Phase 5 — Django web app
- [ ] Phase 6 — Deployment + portfolio

## Author
**Dieu Merci IGABUKWISHAKA** — Year 3 Electrical Power Engineering, University of Rwanda and
Data Science student at ALX Africa
