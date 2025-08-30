# Visualizing Maize Variety Adoption & Agronomic Practices in Embu, Kenya

This project analyzes maize variety adoption and agronomic practices among farmers in **Embu, Kenya** using **Microsoft Power BI**. It converts survey data into a clean, optimized data model and interactive dashboards to answer key business questions around varieties, inputs, constraints, and training effectiveness.

---

## Project Objectives
- Build an **optimized data model** (star schema) for performance and clarity.
- Create **interactive Power BI reports** answering core questions on adoption and practices.
- Quantify the role of **training/extension** in technology uptake.
- Surface **constraints** (e.g., high input costs, pests/diseases) to inform interventions.

---

## Data Modeling Approach
A **Star Schema** was used for efficient slicing and aggregation.

**Dimension Tables**
- `Farmer_Dim`: `HouseholdID`, `Gender`, `County`
- `Variety_Dim`: `VarietyID`, `VarietyName`, `Type`
- `Training_Dim`: `TrainingSourceID`, `SourceName`
- `Practice_Dim`: `PracticeID`, `PracticeName`

**Fact Table**
- `Adoption_Fact`: `HouseholdID`, `VarietyID`, `PracticeID`, `TrainingSourceID`, constraint flags (e.g., `HighCost`, `PestsDiseases`, etc.)

This design reduces redundancy, simplifies DAX, and speeds up visuals.

---

## Dashboards & Key Visuals
- **Socio-economic profile** (gender, age, education, household size, land tenure)
- **Training reach & sources** (extension, NGOs, agro-dealers, media, peers)
- **Land use** (maize land ratio, availability)
- **Variety adoption** (most/least common varieties; improved vs local)
- **Input adoption** (fertilizer type & timing; crop protection)
- **Constraints heatmap** (high cost, pests/diseases, weather, seed/fertilizer quality, post-harvest)
- **Practices by gender** (tillage & weeding)

---

## Screenshots
- ![Screenshot 974](Screenshot%20(974).png)
- ![Screenshot 975](Screenshot%20(975).png)
- ![Screenshot 976](Screenshot%20(976).png)
- ![Screenshot 977](Screenshot%20(977).png)

---

## Findings: Visualizing Maize Variety Adoption and Agronomic Practices in Embu, Kenya

### 1️Socio-economic Dashboard
- **Total Farmers by Gender of Household Head**
  - Male-headed households: **117 (78.52%)**
  - Female-headed households: **32 (21.48%)**
- **Average Age of Farmers:** ~54 years  
- **Average Household Size:** ~7 members  
- **Education Levels:**
  - Primary: 40 farmers
  - Secondary: 60 farmers
  - College/University: 20 farmers
- **Land Ownership:** Majority own land, with some hired or unspecified tenure.

### 2️⃣ Training and Land Usage Dashboard
- **Training Received:**
  - Trained: **109 farmers (73.15%)**
  - Not Trained: **40 farmers (26.85%)**
- **Sources of Training/Advice:** Extension officers, NGOs, agro-dealers, other farmers, and media.
- **Land Use & Availability:**
  - Average maize land ratio: **0.73**
  - Training positively correlated with maize land use.

### 3️⃣ Variety and Fertilizer Usage Dashboard
- **Fertilizer Usage:**
  - Inorganic: **91 farmers (61.07%)**
  - Organic: **36 farmers (24.16%)**
  - Both: **4 farmers (2.68%)**
- **Most Common Varieties:** H6213, H513, WH505, H516, DK8031, Pioneer 38, H614D, Tembo 73, DK777, H624, H628, and local seed.
- **Improved Varieties Adoption:**
  - Yes: **144 (96.6%)**
  - No: **5 (3.4%)**
- **Fertilizer Application Periods:** Basal, Top dressing, and Both (varies by farmer).
- **Identifying Improved Varieties:**
  - Most informed by extension, NGOs, or other farmers.
  - A small proportion could not identify improved varieties.

### 4️⃣ Constraints, Tillage, and Weeding Methods Dashboard
- **Key Constraints Reported:**
  - High cost of inputs
  - Pests & diseases
  - Unpredictable weather
  - Poor seed quality
  - Poor fertilizer quality
  - Post-harvest losses
- **Tillage Methods:** Ploughing and minimum tillage dominant.
- **Weeding Methods:** Hand weeding most common, with some use of herbicides or other methods.

### Observations
- Male-headed households dominate maize production in Embu.
- Training significantly influences adoption of improved varieties and input use.
- Improved maize varieties (especially **H6213** and **H513**) are widely adopted.
- Fertilizer usage is relatively high, but application methods vary.
- Farmers face multiple production constraints, with **input costs and pests** being most severe.
- Traditional practices (ploughing, hand weeding) still dominate, though modern methods are emerging.

---

## Recommendations
1. **Targeted input support:** Consider seed/fertilizer vouchers or seasonal subsidies to ease **high input cost** constraints.
2. **Scale up extension & peer learning:** Expand **extension officer** outreach and structured **farmer-to-farmer** trainings; prioritize practical demos on fertilizer timing and crop protection.
3. **Promote resilient varieties:** Emphasize improved, locally adapted varieties (e.g., drought/pest-tolerant) with verified certification channels.
4. **Quality assurance:** Strengthen seed/fertilizer **quality control** and farmer awareness on identifying certified inputs.
5. **Integrated pest management (IPM):** Train on IPM to reduce losses and costs, combining cultural, biological, and safe chemical methods.
6. **Post-harvest handling:** Provide training and access to **drying/storage** solutions to reduce post-harvest losses.
7. **Gender-responsive programming:** Ensure training schedules, locations, and content are accessible to **female-headed households**.
8. **Monitoring dashboard:** Keep this Power BI dashboard updated to track adoption, constraints, and training effectiveness over time.

---
