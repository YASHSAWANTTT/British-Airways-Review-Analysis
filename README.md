
# ✈️ British Airways Review Analysis (2016–2023)

This project presents an interactive Tableau dashboard analyzing **British Airways passenger reviews** from **March 2016 to October 2023**, using a combination of user feedback metrics, aircraft data, travel types, and geographical context. It offers insights into passenger sentiment, aircraft performance, and regional satisfaction trends.

## 🔗 Live Dashboard

<div class='tableauPlaceholder' id='viz1743709655027' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Bo&#47;Book1_17437090147830&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='Book1_17437090147830&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Bo&#47;Book1_17437090147830&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>
<script type='text/javascript'>
    var divElement = document.getElementById('viz1743709655027');
    var vizElement = divElement.getElementsByTagName('object')[0];
    if ( divElement.offsetWidth > 800 ) {
        vizElement.style.width='1200px';vizElement.style.height='727px';
    } else if ( divElement.offsetWidth > 500 ) {
        vizElement.style.width='1200px';vizElement.style.height='727px';
    } else {
        vizElement.style.width='100%';vizElement.style.height='1477px';
    }
    var scriptElement = document.createElement('script');
    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
    vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>

---

## 🧩 Problem Statement

In the competitive airline industry, customer satisfaction is critical to loyalty and brand perception. However, airlines often struggle to **identify which aspects of the travel experience influence ratings the most** and **how these experiences vary across aircraft, traveler types, and regions**.

**This project aims to solve:**
> _"How can British Airways understand patterns in customer satisfaction and identify operational factors affecting low ratings to improve overall passenger experience?"_

---

## 📂 Dataset

### 1. `ba_reviews.csv`
- Contains over 1,000 user reviews from verified and non-verified flyers.
- Key Columns:
  - `rating`: Overall user rating (1 to 5)
  - `cabin_staff_service`, `seat_comfort`, `entertainment`, etc.
  - `traveller_type`, `seat_type`, `aircraft`, `place`, `route`, and `recommended`

### 2. `Countries.csv`
- Provides mapping of countries to **continent** and **region**.
- Used to enable continental and geographical filtering in the dashboard.

---

## 📊 Key Features of the Dashboard

### 🔹 KPI Metrics
At the top, the dashboard highlights average ratings across 7 features:
- **Overall Rating:** 4.2
- **Cabin Staff Service:** 3.3
- **Entertainment:** 1.4
- **Food & Beverages:** 2.4
- **Ground Service:** 3.0
- **Seat Comfort:** 2.9
- **Value for Money:** 2.8

### 🔹 Filters
The left panel allows filtering by:
- **Metric** (any of the rating categories)
- **Date range**
- **Continent**
- **Aircraft Type**
- **Seat Type** (Business, Economy, etc.)
- **Traveller Type** (Solo, Couple, Family, etc.)

### 🔹 Visuals
1. **Average Rating Over Time**
2. **Average Rating by Country**
3. **Average Rating by Aircraft**
4. **Review Count by Aircraft**

---

## 🧠 Project Analysis & Insights

### ✈️ 1. Aircraft Type Impacts Experience
- **Top-rated aircraft**: Boeing 747-400 (Avg. Rating: 4.7)
- **Low-rated aircraft**: A321 (Avg. Rating: 3.6)

### 🌍 2. Regional Patterns
- High review volume from UK, US, and Australia.
- Some countries in Europe and Asia show dissatisfaction.

### 📆 3. Time-based Trends
- Clear dip in 2020–2021 due to the COVID-19 pandemic.

### 👩‍✈️ 4. Cabin Staff vs In-Flight Features
- Cabin staff scored the highest (3.3).
- Entertainment and Value for Money were the lowest.

### 🪑 5. Seat Type & Traveller Type
- Business and Couple Leisure travelers reviewed most often.

### 🧮 6. Volume vs Satisfaction
- High review count ≠ High satisfaction (e.g., A320).

---

## ✅ Key Conclusions

- Entertainment systems and seating comfort need urgent improvement.
- Extend high long-haul service quality to short-haul routes.
- Understand traveler-specific expectations and tailor services.
- Use aircraft performance insights in strategic fleet planning.

---

## 🛠 Tools Used

| Tool       | Purpose                                  |
|------------|------------------------------------------|
| **Tableau** | Building the interactive dashboard       |
| **Excel/CSV** | Data preprocessing and cleaning        |
| **Python**  | (Optional) Initial data exploration      |
| **GitHub** | Project documentation and hosting        |

---

## 🧼 Data Cleaning Notes

- Cleaned missing `entertainment` values (-1).
- Merged place and country data using `Countries.csv`.
- Normalized aircraft values and dealt with inconsistent labels.

---

## 🚀 How to Reproduce

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/british-airways-dashboard.git
   ```

2. Open Tableau Desktop or Public.

3. Load `ba_reviews.csv` and `Countries.csv`.

4. Join datasets and replicate visuals.

---

## 📎 Future Improvements

- Add NLP-based sentiment analysis on review text.
- Split verified vs unverified traveler experiences.
- Implement dashboard auto-refresh with new data.

---

## 📬 Contact

Made by **[Atharva Yashwant Gadhave](https://yashsawant.dev/)**  
Feel free to connect via [LinkedIn](https://www.linkedin.com/in/yourprofile) or raise issues on GitHub.
