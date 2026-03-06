# Flights Delay Prediction

**MGMT 590 — Big Data Analytics & MLOps**

Predicting whether a flight will be delayed (>15 minutes) using US flight data (2019–2023) and Spark MLlib on Databricks.

---

## 📁 Project Deliverables

| File | Description |
|------|-------------|
| `(Clone) DataCleaningandAnalysis.ipynb` | Main notebook — data prep, EDA, modeling (LR, RF, XGBoost, LightGBM), MLflow |
| `presentation_updated.pptx` | Project presentation slides |
| `report_updated.docx` | Phase 4–5 report with methodology and results |

---

## 📊 Dataset

- **Source:** US domestic flights (2019–2023)
- **Sample:** ~3M rows (`flights_sample_3m.csv`)
- **Features (pre-departure):** AIRLINE, ORIGIN, DEST, MONTH, DAY_OF_WEEK, DEP_HOUR, DISTANCE
- **Label:** 1 if DEP_DELAY > 15 min, else 0

---

## 🛠️ Tech Stack

- **Platform:** Databricks (Spark)
- **ML:** PySpark MLlib, XGBoost, LightGBM, scikit-learn
- **Tracking:** MLflow

---

## 🚀 How to Run

1. **Databricks:** Open the notebook in a Databricks workspace
2. **Data path:** Update the CSV path if needed:
   ```
   /Volumes/workspace/default/bigdataproject/flights_sample_3m.csv
   ```
3. **Run order:** Execute cells top to bottom
4. **XGBoost/LightGBM:** Run `%pip install xgboost lightgbm scikit-learn` before the extended Phase 4 cells

---

## 📈 Models & Results

| Model | AUC | Notes |
|-------|-----|------|
| Logistic Regression | ~0.65 | Baseline |
| Random Forest | ~0.65 | 100 trees, depth 10 |
| Tuned Random Forest | ~0.65 | 200 trees, depth 15 |

---

## 📂 Repository Structure

```
.
├── README.md
├── (Clone) DataCleaningandAnalysis.ipynb
├── presentation_updated.pptx
├── report_updated.docx
├── Phase4_XGBoost_LightGBM.py
├── Phase4_Model_Improvements.py
└── XGBoost_LightGBM_INSTRUCTIONS.md
```

---

## 👥 Authors

MGMT 590 Project Team
