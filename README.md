# 🚀 SpaceX Launch Analysis and Prediction  
This project analyzes SpaceX rocket launch data to identify key factors influencing launch success and predict future outcomes. The project includes data collection, cleaning, exploratory analysis, interactive visualizations, and machine learning model development to forecast launch success.  

## 📌 **Project Overview**  
The goal of this project is to predict the success of SpaceX rocket landings and understand the factors influencing launch outcomes. By analyzing payload mass, launch site, and orbit type, the project provides insights into SpaceX's operational efficiency and reusability strategies.  

## 💡 **Key Features**  
✅ Web scraping to collect launch data from public sources  
✅ Data cleaning and preprocessing using Python (Pandas)  
✅ SQL-based data exploration for key insights  
✅ Interactive dashboards using Plotly Dash and Folium  
✅ Machine learning model (Random Forest) for success prediction (~87% accuracy)  

## 🚀 **Project Structure**  
### **1. Lab 1: Collecting the Data**  
- Collected data from the SpaceX REST API and additional public sources.  
- Used Python's `requests` library to make HTTP GET requests and extract key fields like `launch_date`, `payload_mass`, `orbit`, `launch_site`, and `success`.  
- Ensured structured data retrieval with high accuracy and minimal data loss.  
- **Goal:** Create a comprehensive dataset of SpaceX launch data for analysis.  

### **2. Lab 2: Finishing Web Scraping**  
- Performed web scraping using Python libraries `BeautifulSoup` and `Requests`.  
- Extracted additional information from SpaceX-related public websites and news sources.  
- Parsed HTML content to extract key insights about payloads, launch locations, and outcomes.  
- Cleaned and stored the extracted data using `Pandas`.  
- **Goal:** Supplement API data with external contextual data to improve analysis.  

### **3. Lab 3: Data Wrangling**  
- Cleaned and organized the dataset to prepare it for analysis and modeling.  
- Handled missing values using interpolation and mean-based imputation.  
- Removed duplicates and standardized data types (e.g., payload values converted to floats).  
- Created new features to improve model performance (e.g., payload categories, booster version).  
- **Goal:** Create a clean and structured dataset ready for analysis and modeling.  

### **4. Lab 4: SQL Notebook**  
- Performed SQL-based analysis to identify patterns and trends in the data.  
- Created queries to analyze launch success rates, payload mass, and orbit-specific performance.  
- Grouped data by launch site and customer to identify consistent success patterns.  
- Provided foundational insights for subsequent visualizations and modeling.  
- **Goal:** Extract meaningful insights from structured data to support exploratory analysis.  

### **5. Lab 5: Exploring and Preparing Data**  
- Conducted exploratory data analysis (EDA) using `Matplotlib` and `Seaborn`.  
- Created visualizations to explore the relationships between payload mass, orbit type, and success rate.  
- Found that lower payload masses correlated with higher success rates.  
- Discovered that certain orbit types (e.g., LEO) had consistently higher success rates.  
- **Goal:** Establish foundational insights to guide dashboard creation and modeling.  

### **6. Lab 6: Interactive Visual Analytics with Folium**  
- Developed an interactive map using `Folium` to visualize launch sites and success rates.  
- Plotted launch site markers and used different colors to represent successful and failed launches.  
- Added circles to represent launch site proximity to infrastructure (e.g., highways, coastlines).  
- Included trajectory lines to visualize flight paths.  
- **Goal:** Provide a geographic understanding of launch outcomes and site-specific performance.  

### **7. Lab 6 Part 2: Plotly Dash App**  
- Built an interactive dashboard using `Plotly Dash` to analyze payload and launch success.  
- Added a dropdown to filter by launch site and a range slider to adjust payload mass.  
- Created a pie chart to display success rates by site and a scatter plot to show payload-success correlation.  
- Ensured real-time updates based on user input.  
- **Goal:** Provide an intuitive interface for exploring launch success patterns dynamically.  

### **8. Lab 7: Machine Learning Prediction**  
- Developed and compared several classification models:  
   - Logistic Regression  
   - Decision Tree  
   - Random Forest  
   - Gradient Boosting  
- Used `GridSearchCV` to tune hyperparameters and optimize model performance.  
- Best model: **Random Forest** with ~87% accuracy.  
- Handled class imbalance using Synthetic Minority Over-sampling Technique (SMOTE).  
- Evaluated performance using:  
   - Accuracy – Percentage of correct predictions.  
   - F1 Score – Balance between precision and recall.  
   - Confusion Matrix – Identified false positives/negatives.  
- **Goal:** Build a high-performance predictive model for launch success.  

## 📈 **Results and Insights**  
### **Exploratory Analysis Insights:**  
- Success rates were highest for low-payload launches, especially for payloads under **4,000 kg**.  
- Specific launch sites (e.g., **KSC LC-39A** and **CCAFS SLC-40**) consistently outperformed others.  
- Orbit type and payload mass were the most influential factors for success:  
   - Low Earth Orbit (LEO) had the highest success rates due to lower energy requirements.  
   - High orbits (e.g., GEO) had lower success rates due to more complex launch conditions.  
- Success rate increased significantly after **2015** due to improvements in rocket design and reusable boosters.  
- Higher flight numbers (experience) were correlated with higher success rates.  

### **Dashboard Insights:**  
- Interactive dashboard confirmed that payload mass and orbit type are key success drivers.  
- Drop-down and slider allowed for real-time exploration of site-specific performance and payload correlations.  
- Success rates for low-payload launches were notably higher, consistent with the model’s findings.  
- Successful launches were more frequent from **KSC LC-39A** and **VAFB SLC-4E**.  

### **Machine Learning Insights:**  
- Best Model: **Random Forest** – Achieved 87% accuracy after hyperparameter tuning.  
- Model identified payload mass, orbit type, and launch site as the most important predictors.  
- Confusion Matrix showed high true positive and true negative rates with minimal false negatives.  
- High F1 score indicated that the model balanced precision and recall effectively.  

### **Strategic Insights:**  
- Predicting landing success allows SpaceX to estimate future launch costs more accurately.  
- Identifying the best-performing launch sites and payload categories enables better resource allocation.  
- Success rate improvements post-2015 demonstrate the value of reusable rocket technology.  
- The model’s ability to predict success with high accuracy enables operational and cost optimizations.  

## 🔗 **Links**  
- [GitHub Repository](https://github.com/SamHerd/IBMCapstone)  
- [LinkedIn Profile](https://www.linkedin.com/in/samherd)  

## 👨‍💻 **Author**  
Sam Herd  
[GitHub](https://github.com/SamHerd) | [LinkedIn](https://www.linkedin.com/in/samherd)  
