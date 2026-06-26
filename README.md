# 🎬 Netflix Movies & TV Shows Analysis

## 📊 Project Overview

This project performs a comprehensive **Exploratory Data Analysis (EDA)** on Netflix's catalog of **8,807 titles** (including movies and TV shows). The analysis uncovers critical insights about content strategy, optimal release timing, popular genres, top actors/directors, and viewer preferences to guide content production and release decisions.

**Analysis Period:** Historical Netflix catalog (through 2021)  
**Total Records:** 8,807 titles  
**Key Focus:** Content distribution, ratings, duration patterns, geographic trends, release timing optimization

---

## 🎯 Objectives

- Analyze **content type distribution** (movies vs. TV shows) and their respective characteristics
- Identify **optimal release timing** for movies and TV shows (best months, weeks)
- Examine **rating patterns** and audience targeting (TV-MA, PG, etc.)
- Study **geographic content production** trends across countries
- Analyze **top actors and directors** in Netflix's catalog
- Explore **genre popularity** and content category distribution
- Understand **content duration patterns** (movie length, TV show seasons)
- Correlate **release timing** with content success metrics

---

## 🛠 Tools & Technologies Used

| Tool | Purpose |
|------|---------|
| **Python 3.x** | Core programming language for data analysis |
| **Pandas** | Data manipulation, aggregation, and transformation |
| **NumPy** | Numerical operations and array processing |
| **Matplotlib** | Data visualization and plotting |
| **Seaborn** | Advanced statistical visualization |
| **Plotly** | Interactive visualizations |
| **WordCloud** | Text visualization for genre and content analysis |

---

## 📁 Dataset Information

### Dataset Source
**Kaggle:** Netflix Shows Dataset  
Link: [Netflix Shows on Kaggle](https://www.kaggle.com/shivamb/netflix-shows)

### Dataset Structure
```
Total Records: 8,807 Netflix titles
Total Columns: 12 attributes per title
File Format: CSV
```

### Column Descriptions

| Column | Type | Description |
|--------|------|-------------|
| **show_id** | String | Unique identifier for each title |
| **type** | String | "Movie" or "TV Show" |
| **title** | String | Name of the show/movie |
| **director** | String | Director(s) of the content |
| **cast** | String | Main cast members |
| **country** | String | Production country(s) |
| **date_added** | DateTime | Date content was added to Netflix |
| **release_year** | Integer | Original release year |
| **rating** | String | Content rating (TV-MA, PG, etc.) |
| **duration** | String | Movie duration (minutes) or TV seasons count |
| **listed_in** | String | Genre(s) classification |
| **description** | String | Brief plot summary |

---

## 🔍 Analysis Methodology

### 1. **Data Cleaning & Preparation**
- Handle missing values strategically (replace with "Unknown" where appropriate)
- Convert data types for temporal analysis
- Split composite columns (director, cast, country) for granular analysis
- Remove duplicates and validate data integrity

### 2. **Content Distribution Analysis**
- Calculate movie vs. TV show proportions
- Analyze duration patterns
- Study rating distributions

### 3. **Temporal Analysis**
- Extract temporal features (day, week, month, year added)
- Identify seasonal release patterns
- Determine optimal release windows

### 4. **Geographic Analysis**
- Parse multi-country productions
- Rank countries by content production
- Analyze production trends

### 5. **Cast & Crew Analysis**
- Parse and explode actor/director lists
- Rank top performers by content count
- Identify prolific creators

### 6. **Genre Analysis**
- Parse and categorize multiple genres per title
- Rank genres by popularity
- Visualize genre trends

---

## 📈 Key Findings

### **Content Distribution**
- **Total Movies:** 6,131 (69.62%)
- **Total TV Shows:** 2,676 (30.38%)
- **Most common rating:** TV-MA (adult audience focus)

### **Top Content Producers**
| Country | Movies | TV Shows |
|---------|--------|----------|
| United States | 2,751 | 938 |
| India | 962 | - |
| United Kingdom | 532 | 272 |
| Japan | - | 199 |

### **Optimal Release Timing**
#### For TV Shows:
- **Best Week:** First week of the month
- **Best Month:** October
- **Best Year:** 2021 (highest production volume)

#### For Movies:
- **Best Week:** First week of the month
- **Best Months:** January, April, July
- **Best Year:** 2021 (followed by 2019)

### **Content Duration**
- **Average Movie Length:** 90-120 minutes
- **Most Common TV Duration:** Single season (1 season)

### **Top Performers**
| Category | Name | Count |
|----------|------|-------|
| **Top Actor** | Anupam Kher | 39 titles |
| **2nd Top Actor** | Rupa Bhimani | 31 titles |
| **Top Director** | Rajiv Chilaka | Multiple titles |
| **Most Popular Genre** | International Movies | Highest frequency |
| **2nd Popular Genre** | Dramas | High frequency |

### **Rating Insights**
- Majority of content targets adult audiences (TV-MA rating dominates)
- Limited family-friendly content in premium spots
- Seasonal spikes in specific genres

---

## 💡 Business Insights & Recommendations

### 1. **Strategic Market Focus**
✅ Maintain investment in US, India, and UK as primary production hubs  
✅ Expand operations in emerging markets like Japan  
✅ Consider localization strategies for regional preferences

### 2. **Content Strategy Optimization**
✅ Prioritize adult-oriented dramas and thrillers  
✅ Increase production in popular genres (International movies, Dramas)  
✅ Consider niche content gaps for family entertainment

### 3. **Release Timing Strategy**
✅ **TV Shows:** Launch in October, first week of month for maximum visibility  
✅ **Movies:** Plan releases for January, April, July windows  
✅ Avoid oversaturation during peak periods

### 4. **Talent Acquisition**
✅ Spotlight top actors (Anupam Kher, Rupa Bhimani) in promotional campaigns  
✅ Partner with prolific directors like Rajiv Chilaka for flagship projects  
✅ Scout emerging talent in high-performing regions

### 5. **Content Library Management**
✅ Maintain 70% movies to 30% TV shows ratio  
✅ Balance adult content with family-friendly options  
✅ Regular refresh cycles aligned with optimal release periods

---

## 🔄 How to Use This Analysis

1. **View the Report:** Open the [PDF Report](Netflix%20Data%20Exploration%20Business%20Case2.ipynb%20-%20Colab.pdf) for detailed findings and visualizations
2. **Review the Code:** Check `netflix_data_exploration_business_case1.py` for implementation details
3. **Reproduce Results:** Run Python scripts with your own data
4. **Adapt Methodology:** Use analysis approach for other streaming platforms

---

## 📊 Deliverables

| File | Description | Size |
|------|-------------|------|
| 📄 **PDF Report** | Comprehensive analysis with visualizations | 1.9 MB |
| 🐍 **Python Script** | Executable analysis code | 19.4 KB |
| 📋 **README** | This documentation file | - |

---

## 🚀 Future Enhancements

- [ ] Add interactive Tableau/Power BI dashboards
- [ ] Implement predictive modeling for content success
- [ ] Create recommendation engine based on genres/ratings
- [ ] Add sentiment analysis on descriptions
- [ ] Real-time data pipeline integration
- [ ] Comparative analysis with competitor platforms

---

## 📝 Technical Notes

### Data Quality
- **Missing Values:** Strategically handled using "Unknown" replacement
- **Data Types:** Converted appropriately for analysis
- **Temporal Data:** Parsed from various date formats

### Analysis Limitations
- Analysis based on static snapshot (up to 2021)
- Some multi-country productions may be undercounted
- Cast/director data may have formatting inconsistencies

### Performance Metrics
- Processing Time: Optimized for 8,807 records
- Memory Efficient: Pandas groupby operations for aggregations
- Visualization Quality: High-resolution charts for presentation

---

## 👨‍💼 Author & Contact

**Name:** Sanjesh Chourasia  
**GitHub:** [@Sanjesh12](https://github.com/Sanjesh12)  
**Project Type:** Exploratory Data Analysis & Business Case Study  
**Difficulty Level:** Intermediate to Advanced  

---

## 📜 License

This project is available for educational and professional reference purposes. Feel free to adapt the methodology for your own streaming data analysis.

---

## 🙏 Acknowledgments

- **Data Source:** Kaggle Community (Netflix Shows Dataset)
- **Inspiration:** Netflix's content strategy and market positioning
- **Tools:** Python open-source community

---

**Last Updated:** September 2025  
**Status:** ✅ Analysis Complete | 🔄 Continuously Updated  
**Next Review:** Q4 2025

