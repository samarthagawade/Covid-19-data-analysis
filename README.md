# 🧬 COVID-19 Clinical Trials Data Analysis

## 📖 **Project Overview**
This project analyzes a dataset of global **COVID-19 clinical trials** to uncover trends in research activity, country-wise participation, gender representation, and trial progress.  
Using Python-based data analysis and visualization, the study explores how the world responded scientifically during the COVID-19 pandemic through large-scale clinical studies.

---

## 🎯 **Objective**
The primary goals of this project are:
- To clean and preprocess COVID-19 clinical trial data.
- To identify countries leading in COVID-19 research.
- To study the distribution of trial statuses (Completed, Recruiting, etc.).
- To analyze gender-based participation patterns.
- To determine which months had the highest number of trial initiations.
- To visualize the findings through charts and graphs for better understanding.

---

## 📊 **Dataset Description**
- **Dataset Name:** `COVID clinical trials.csv`
- **Source:** ClinicalTrials.gov (or similar open-source dataset)
- **Type:** Tabular dataset representing clinical studies conducted worldwide.
- **Size:** Several thousand records of clinical trials related to COVID-19.

### **Key Columns:**
| Column | Description |
|--------|--------------|
| **Rank** | Index number or identifier of each clinical trial |
| **Status** | Shows progress of the trial (Completed, Recruiting, Terminated, etc.) |
| **Gender** | Indicates whether the trial included Male, Female, or Both participants |
| **Enrollment** | Number of participants enrolled |
| **Locations** | Geographic regions or countries where trials were conducted |
| **Start Date** | Date when the trial was initiated |
| **Study Documents / Results First Posted** | Removed due to irrelevance or redundancy |

---

## ⚙️ **Methodology**
### **1. Data Cleaning**
- Loaded dataset using `pandas`.
- Dropped unnecessary columns (`Results First Posted`, `Study Documents`).
- Removed duplicate entries.
- Handled missing values:
  - Replaced missing numeric values (`Enrollment`) with median.
  - Replaced missing categorical values with `"None"`.
- Created a new **Country** column derived from the `Locations` field.
- Set `Rank` as the index column.

### **2. Feature Engineering**
- Converted `Start Date` into datetime format.
- Extracted `Start Month` from `Start Date` for time-based trend analysis.

### **3. Data Visualization**
Generated various bar charts using **Matplotlib** and **Pandas plotting**:
- **Top 10 Countries** contributing most trials.  
- **Status Distribution** of all clinical trials.  
- **Gender Distribution** among participants.  
- **Monthly Trend** of trial start dates.

### **4. Data Export**
- Cleaned dataset was saved as `COVID-19 cleaned.csv` for future use.

---

## 📈 **Key Findings**
1. **Top Contributing Countries:**  
   - The **USA**, **China**, and **India** lead the world in conducting COVID-19 trials.  
   - Developed and emerging nations contributed significantly to global research.

2. **Trial Status:**  
   - Most trials were **Completed** or **Recruiting**, showing steady global research activity.  
   - Very few trials were terminated or withdrawn.

3. **Gender Representation:**  
   - Majority of trials involved **both genders**, promoting inclusivity.  
   - Few gender-specific studies were conducted for biological focus areas.

4. **Enrollment Patterns:**  
   - Trials varied in scale, with enrollment ranging from small groups to large-scale studies.  
   - Median imputation ensured numerical consistency.

5. **Monthly Trends:**  
   - Most trials began between **April and August 2020**, correlating with the initial global outbreak period.  
   - Reflects the urgency and immediate scientific response to the pandemic.

---

## 🧠 **Conclusion**
This analysis highlights the global collaboration and rapid mobilization of research during the COVID-19 pandemic.  
Key takeaways include:
- Global cooperation among countries in medical research.  
- High proportion of completed studies reflecting commitment and progress.  
- Balanced gender representation in study design.  
- Surge in research activity during the early pandemic months.

### **Future Scope**
- Perform correlation analysis between country contributions and trial success rates.  
- Use machine learning models to predict completion times or study outcomes.  
- Conduct text or sentiment analysis on study summaries to identify common research themes.

---

## 🧰 **Technologies Used**
- **Python**  
- **Pandas**  
- **NumPy**  
- **Matplotlib**  
- **Scikit-learn**  
- **Google Colab**

---

 for educational and research purposes.
