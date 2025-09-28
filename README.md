# 🏡 Intelligent Data Collection Framework for House Cost Prediction

This project presents a robust and intelligent framework to **automate house price prediction** by integrating real-time property listings, geospatial data, and multiple machine learning models. It enhances the accuracy of real estate valuations using a combination of structured web data, location context, and ensemble modeling techniques.

---

## 📌 Project Overview

Traditional property valuation methods often rely on outdated data and manual analysis, which limits their accuracy and adaptability. This framework:

- Automates the collection of housing data using **web scraping**.
- Enhances listings with **geospatial data** from APIs.
- Performs **feature engineering** to extract meaningful variables.
- Applies and compares **multiple regression models**.
- Provides a **user-friendly web interface** for live predictions.

---

## 🔍 Key Features

- 🗂️ **Comprehensive Data Collection**: Scrapes property listings with size, location, rooms, type, and pricing info.
- 🌐 **API Integration**: Uses Google Maps API to gather nearby amenities (schools, parks, hospitals).
- 🧼 **Data Standardization & Cleaning**: Normalizes and transforms messy data, handles missing values.
- 📊 **Advanced Feature Engineering**: Adds distance metrics, construction year, renovation year, etc.
- 🤖 **ML Models & Ensemble Learning**:
  - Linear Regression
  - Random Forest
  - Gradient Boosting
  - LightGBM
  - Voting Regressor (ensemble)
- 🧪 **Performance Evaluation**: MAE, RMSE, R² Score, log-transformed metrics
- 🌍 **Web Interface**: Built using Flask and Streamlit for interactive predictions
- 📈 **Visualizations**: Geospatial heatmaps, feature importance (SHAP), trends

---

## 📊 Model Performance

| S.no | Model Name             | MSE  | R² Score |
|------|------------------------|------|----------|
| 1.   | Linear Regression      | 0.45 | 0.509    |
| 2.   | Random Forest Regressor| 0.08 | 0.915    |
| 3.   | Gradient Boosting      | 0.21 | 0.768    |
| 4.   | LightGBM               | 0.11 | 0.878    |
| 5.   | Voting Regressor       | 0.11 | 0.880    |

> ✅ **Best Model**: Voting Regressor (combines Random Forest and Gradient Boosting)

---

## 📂 Data Sources

The framework uses datasets derived from real estate websites and enriched via APIs:

- `final_data.csv` – Main cleaned dataset
- `lat_long.csv` – Location coordinates
- `merged_output.csv` – Final merged dataset
- `output.csv`, `output.xlsx - Sheet1.csv` – Intermediate outputs
- `locations_amenities_list_total.json` – Location-based amenity info

🔗 Access all datasets here:  
[Google Drive Folder](https://drive.google.com/drive/folders/1dHRb-Ta33KHi15L19tu6FLKzrXWI4l41?usp=sharing)

---

## 🧰 Technologies Used

| Category         | Tools / Libraries                          |
|------------------|--------------------------------------------|
| Programming      | Python (Pandas, NumPy, Requests)           |
| Web Scraping     | Selenium, BeautifulSoup                    |
| APIs             | Google Maps API, OpenStreetMap API         |
| Machine Learning | scikit-learn, XGBoost, LightGBM            |
| Visualization    | Matplotlib, Seaborn, Tableau               |
| Web Frameworks   | Flask, Streamlit                           |
| Notebooks        | Jupyter                                    |
| Version Control  | Git                                        |

---

## 🛠 Project Files

- `scrape.ipynb` – Web scraping of listings  
- `preprocessing1.ipynb` – Data cleaning & transformation  
- `modeltest.ipynb`, `final.ipynb`, `test.ipynb` – ML models & evaluation  
- `merged_output.csv`, `lat_long.csv`, `final_data.csv` – Cleaned datasets  
- `locations_amenities_list_total.json` – API enriched location info  

---

## 🧠 Future Enhancements

- 📡 Real-time listing integration
- 🤖 Deep learning with textual property descriptions
- 🧠 AI-powered feature selection
- 📱 Mobile app version
- 🌐 Global region expansion

---

## 🚧 Challenges Faced

- Missing data for some regions (e.g., New York City)
- Inconsistent data formats across sources
- Continuous scraping and data refresh needs
- Hyperparameter tuning for optimal model accuracy

---

## 👨‍💻 Authors

- **Y. Manikanta** 


## 📜 License

This project is intended for academic and educational purposes only.  

---

## 📞 Contact & Contributions

We welcome contributions and feedback!  
Feel free to fork the repo, raise issues, or submit pull requests.

📧 Contact Emails:
- manikantayeduri0528@example.com


---

## 🙏 Acknowledgements

We sincerely thank **Dr. Mahendra Prasad** for his expert guidance and feedback throughout the project.  
We also acknowledge the support of the **GITAM School of Technology** and our peers for their contributions.

---

## 📚 References

1. Zhang, Y., & Wang, J. (2023). *House price prediction with textual description data.*
2. Liu, X. (2013). *Spatial and Temporal Dependence in House Price Prediction.*
3. Hjort, A., Scheel, I. (2024). *LitBoost: Locally Interpretable Tree Boosting.*
4. Raga Madhuri, et al. (2019). *Regression Techniques: A Comparative Study.*

---

## ⭐ Final Thoughts

This framework delivers a scalable, accurate, and modular solution for real estate price prediction. It blends automation, geospatial analytics, and ensemble learning into a practical tool for real-world property valuation.

> ⭐ If you found this project useful, give it a star and share it with your network!

