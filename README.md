# 🌍 GDP Data Analysis (1960–2016)

This project focuses on analyzing global **GDP data from 1960 to 2016** using Python and pandas. The dataset provides annual GDP values for various countries and regions. The main objective is to compute GDP growth, examine trends, and visualize India’s GDP performance over the years.

---

## 📁 Dataset

**File:** `gdp.csv`

**Columns:**

- `Country Name`: Name of the country or region  
- `Country Code`: ISO 3-letter country code  
- `Year`: Year of the GDP record  
- `Value`: GDP in current US dollars

---

## ✅ Objectives

- Understand the structure and content of the dataset  
- Filter and explore GDP data for specific countries (e.g., India, World)  
- Calculate year-over-year GDP growth percentages  
- Create visualizations of GDP growth trends using plots

---

## 📊 Features

- Calculates **annual GDP growth** for each country  
- Adds a new column `GDP` to represent growth percentage  
- Filters GDP data specifically for **India**  
- Uses **matplotlib** and **seaborn** for clean, readable visualizations

---

## 🛠️ Tools & Libraries

- Python 3.x  
- pandas  
- matplotlib  
- seaborn  
- Jupyter Notebook or any Python IDE

---

## 📈 Sample Visualization

A **line chart** showing India's GDP growth from 1960 to 2016.

```python
import matplotlib.pyplot as plt
import seaborn as sns

india_data = df[df['Country Name'] == 'India']
plt.figure(figsize=(12, 6))
sns.lineplot(data=india_data, x='Year', y='GDP')
plt.title("India's GDP Growth (1960–2016)")
plt.xlabel("Year")
plt.ylabel("GDP Growth (%)")
plt.grid(True)
plt.show()
