# Cricket Player Dashboard (ESPN Cricket Data)
---

## 📌 Problem Statement  

This dashboard helps cricket fans, analysts, and coaches understand a player’s batting, bowling & fielding performance in detail. By selecting a player through a slicer, all visuals dynamically update to show runs trend, highest scores, strike rate patterns, 4s/6s breakdown, and not-out counts.  

The purpose of this report is to:  
- 🎯 Track a player’s consistency.  
- 💯 Compare scoring patterns (boundaries, strike rate).  
- 🏆 Highlight milestones (50s, 100s, not-outs).  
- 📊 Provide quick insights using KPI cards (highest score, total not outs, matches played).  

This dashboard makes player performance analysis simple and interactive.  

---

## Steps followed  

- **Step 1 : 🌐 Data Source (ESPN Cricinfo)**  
  Loaded player statistics directly from the ESPN Cricinfo website using **Power BI’s Web Connector (Get Data → Web)**.  
  - Selected batting statistics tables.  
  - Cleaned up headers and ensured proper data types.

- **Step 2 : 🧹 Data Cleaning**  
  - Removed special characters (`*`) from *Highest Score* column for numeric analysis.  
  - Created calculated columns:  
    - `HighestScoreNumeric` (numeric high score).  
    - `NotOutFlag` (Out / Not Out).  

- **Step 3 : 🔗 Relationships & Modeling**  
  - Verified Player field relationships so slicer could control all visuals.  
  - Created calculated measures for KPIs (e.g., Total Not Outs, Matches Played, Average Strike Rate).  

- **Step 4 : 🎛️ Created Slicer**  
  Added a Player Name slicer → controls all charts (runs trend, scatter plot, KPIs).  

- **Step 5 : 📊 Visuals Added**  

  - **Donut Chart:** Boundaries (4s vs 6s per player).  
  - **Multi-row Card:** Highest Score and Not Out flag.  
  - **Card KPI:** Total Not Outs, Matches Played, Highest Score.  
  - **Table Visual:** Highest Score + Not Out details.  
  - **Gauge / KPI:** Strike rate indicator.  

- **Step 7 : 🎨 Enhancements**  
  - Used single-select slicer for one player at a time.  
  - Designed clean layout with custom theme.  

- **Step 8 : ☁️ Published Report**  
  Published the dashboard to Power BI Service for sharing and collaboration.

---

## Insights  

From the dashboard, the following inferences can be made:  

### [1] 🔥 Highest Score & Not Outs  
- Highest score (numeric) visible in KPI card.  
- Not Outs shown in Multi-row Card / Table.  

### [2] 🎯 Milestones  
- Bar charts show frequency of 50s & 100s.  
- Distribution of 4s and 6s highlights batting style.  

### [3] 🏏 Quick KPIs  
- Total Matches Played  
- Total Not Outs  
- Highest Score  
- Strike Rate  

All KPIs are player-specific and update dynamically based on slicer selection.  

---

✅ A single-page dashboard was created in Power BI Desktop & then published to Power BI Service.  

👉 This makes cricket performance analysis **interactive, visual, and data-driven**. 
