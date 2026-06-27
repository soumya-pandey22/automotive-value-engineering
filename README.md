# Car Purchase Preference Analyzer

A data-driven decision support project built in Python that analyzes car purchasing preferences based on primary survey data collected from 47 respondents. The project applies a weighted scoring framework to rank 9 cars across 7 key parameters, providing actionable insights for both customers and automotive marketers.

---

## Motivation

Buying a car involves trade-offs across multiple factors — safety, fuel efficiency, cost, aesthetics, and more. Different customers prioritize these differently. This project builds a structured analytical framework that quantifies these preferences and maps them to real car ratings, producing an objective ranking system.

---

## Dataset

Three CSV files form the backbone of this project:

| File | Description |
|---|---|
| `survey_preferences.csv` | Parameter importance ratings collected from 47 respondents |
| `car_ratings.csv` | Ratings for 9 cars across 7 parameters on a scale of 1-10 |
| `brand_weights.csv` | Pairwise comparison weights for Tata Motors, Maruti Suzuki and Kia |

**Cars analyzed:** Tata Nexon, Tata Altroz, Tata Tigor, Maruti Grand Vitara, Maruti Breeza, Maruti Ciaz, Kia Sonet, Kia Carens, Kia Seltos

**Parameters:** Safety, Fuel Efficiency, Maintainability, Durability, Manoeuvrability, Cost, Aesthetics

---

## Project Structure
Minor Project/

│

├── analysis.ipynb          # Main Jupyter notebook

├── brand_weights.csv

├── car_ratings.csv

└── survey_preferences.csv

---

## Analysis Sections

**Section 1 — Data Loading**
All three datasets are loaded using Pandas and displayed as formatted tables for initial inspection.

**Section 2 — Survey Analysis**
A horizontal bar chart visualizing how 47 respondents rated the importance of each parameter. Safety emerged as the most important factor while Aesthetics ranked lowest.

**Section 3 — Car Ratings Heatmap**
A colour coded heatmap of the full 9×7 ratings matrix. Dark red indicates high ratings, light yellow indicates low ratings. Enables instant pattern recognition across all cars and parameters simultaneously.

**Section 4 — Weighted Scoring Model**
The core of the project. Each car's parameter ratings are multiplied by the corresponding survey weights and summed to produce a final score. This replicates the manual weighted scoring process programmatically, producing an objective ranking of all 9 cars.

**Section 5 — Sensitivity Analysis**
Safety and Fuel Efficiency weights are swapped to simulate a different customer profile. Rankings are recalculated to demonstrate how the framework adapts to different buyer priorities.

---

## Tech Stack

- Python 3.13
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook (VS Code)

---

## Key Findings

- Safety and Fuel Efficiency are the dominant purchasing criteria among surveyed respondents
- Tata Altroz and Maruti Breeza consistently rank highest across multiple customer profiles
- The weighted scoring framework is flexible and can be adapted to any customer priority set

---

## How to Run

1. Clone the repository
2. Open `analysis.ipynb` in VS Code or Jupyter
3. Run all cells in order using `Shift + Enter`

---

Conclusion

This project successfully demonstrates the application of a weighted scoring framework to evaluate and rank cars based on multi-parameter survey data. By combining primary data collection from 47 respondents with structured analytical techniques, the project moves beyond subjective car buying decisions toward a data-driven approach.

The heatmap visualization revealed clear patterns in car ratings across parameters, while the weighted scoring model produced an objective final ranking. The sensitivity analysis further validated the robustness of the framework by demonstrating how rankings shift when customer priorities change — proving that the model is adaptable and not limited to a single buyer profile.

Overall this project bridges the gap between raw survey data and meaningful decision support, and demonstrates how Python-based data analytics can be applied to real world consumer preference problems.

---

## Future Scope

- **Expand the dataset** — Include more car models across segments (SUV, sedan, hatchback) and collect survey data from a larger and more diverse respondent pool

- **Dynamic weight input** — Build an interactive interface where any customer can enter their own priority weights and instantly get a personalized car ranking

- **Machine Learning integration** — Apply clustering algorithms to segment respondents into buyer profiles (safety focused, budget focused, performance focused) and generate profile specific rankings

- **Real time data** — Integrate live car ratings and pricing data from automotive APIs to keep the analysis current and relevant

- **Web deployment** — Deploy the model as a web application using Flask or Streamlit so non-technical users can interact with it directly through a browser

- **Multi-country analysis** — Extend the survey to respondents across different regions to study how cultural and economic factors influence car buying priorities

## Author

Soumya Pandey
Mechanical Engineering, NIT Jamshedpur
Minor Project — Data Analytics
