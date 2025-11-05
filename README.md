# 📊 Nobel Prize Gender Analysis

This project explores gender representation across Nobel Prize categories and decades. Using Python, pandas, and seaborn, it identifies which category had the highest proportion of female laureates and visualizes trends over time.

---

## 🔍 Key Insight

🏆 In the 2020s, the Nobel Peace Prize had the highest proportion of female laureates, with **40% representation**.

---

## 📁 Project Structure

- `notebook.ipynb` — Main analysis notebook
- `data/nobel.csv` — Nobel Prize dataset
- `Nobel_Prize.png` — Supporting image
- `README.md` — Project overview and instructions

---

## 🧮 Methods Used

- Boolean flagging for gender
- Grouping by decade and category
- Calculating proportions with `.mean()`
- Identifying peak representation with `.max()`
- Visualizing trends using `seaborn.lineplot`

---

## 📊 Visualization

The chart below shows how female representation has evolved across Nobel categories by decade.

```python
sns.lineplot(data=df_ratios, x='decade', y='female', hue='category')
