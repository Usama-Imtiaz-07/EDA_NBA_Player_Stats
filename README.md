# **NBA Player Stats Explorer**

## **Project Overview**
This project is a **Streamlit-based web application** that provides insights into **NBA player statistics** from 1950 to 2020. The app scrapes player stats data from [Basketball Reference](https://www.basketball-reference.com/) and allows users to filter and analyze player statistics by **year**, **team**, and **position**. Users can also visualize correlations between statistical categories and download the filtered data for further analysis.

---

## **Features**
1. **Player Statistics Filtering**:
   - Users can select a specific **year** (from 1950 to 2020) to view player stats for that season.
   - Filter player statistics by **team(s)** using a sidebar multiselect dropdown.
   - Filter player statistics by **position(s)** (Center, Power Forward, Small Forward, Point Guard, Shooting Guard).

2. **Data Display**:
   - Displays filtered player statistics in a tabular format, including metrics like points per game, rebounds, assists, and more.

3. **Data Download**:
   - Enables users to download the filtered player stats data as a **CSV file** for offline analysis.

4. **Heatmap Visualization**:
   - Generates an **intercorrelation heatmap** to visualize relationships between different statistical categories (e.g., points, rebounds, assists).

---

## **How It Works**
1. **Data Retrieval**:
   - The app scrapes NBA player stats data from [Basketball Reference](https://www.basketball-reference.com/) using `pandas.read_html`.
   - Data is cached to improve performance when switching between years.

2. **User Interaction**:
   - Users can select a **year**, **team(s)**, and **position(s)** to filter the data.
   - The app dynamically updates the displayed data based on user selections.

3. **Visualization**:
   - The app uses **Seaborn** and **Matplotlib** to generate an intercorrelation heatmap for the selected data.
   - The heatmap provides insights into the relationships between different player statistics.

---

## **Technologies Used**
- **Python Libraries**: Streamlit, Pandas, NumPy, Matplotlib, Seaborn, base64.
- **Data Source**: [Basketball Reference](https://www.basketball-reference.com/).
- **Deployment**: Streamlit (web-based).

---

## **How to Run the App**
1. **Install Dependencies**:
   ```bash
   pip install streamlit pandas matplotlib seaborn numpy
   ```

2. **Run the App**:
   ```bash
   streamlit run app.py
   ```

3. **Access the App**:
   - Open the provided URL in your browser to interact with the app.

---

## **Future Enhancements**
- Add more advanced filtering options, such as filtering by player name or specific statistical thresholds.
- Include additional visualizations, such as bar charts or scatter plots, to explore player stats further.
- Integrate machine learning models to predict player performance or team outcomes.

---

## **Contributors**
- Usama imtiaz
