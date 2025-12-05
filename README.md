# Yelp Data Analysis Project  
**End-to-End Modern Data Pipeline & Interactive Business Intelligence Dashboard**  
Built with Python • AWS S3 • Snowflake • Snowflake • Amazon QuickSight  

<img width="1654" height="894" alt="image" src="https://github.com/user-attachments/assets/3e678263-ff08-4f3d-91b4-8efcbf5d7893" />

## Project Overview
This project demonstrates a **production-grade, cloud-native data pipeline** that ingests, processes, and visualizes the official Yelp Academic Dataset containing **~7 million reviews** and **150K+ businesses**.

### Key Achievements
- Loaded the entire 5 GB raw nested JSON dataset into Snowflake in **under 60 seconds** (vs hours manually)
- Implemented **in-database sentiment analysis** using a Python TextBlob UDF
- Created **two fully interactive Amazon QuickSight dashboards** powered by 10 advanced SQL queries
- Delivered actionable insights on geography, categories, sentiment, and trends

## Tech Stack
| Component       | Technology                  |
|-----------------|-----------------------------|
| Processing      | Python 3.9+                 |
| Storage         | Amazon S3                   |
| Data Warehouse  | Snowflake (VARIANT + FLATTEN) |
| NLP             | TextBlob UDF in Snowflake   |
| SQL Analytics   | CTEs, Window Functions, RANK/DENSE_RANK |
| Visualization   | Amazon QuickSight           |

## Architecture
<img width="1539" height="756" alt="image" src="https://github.com/user-attachments/assets/e1d870ef-7502-4712-9d81-60b5601f8bcd" />


## Dataset Summary
| Metric                     | Value                  |
|--------------------------------|------------------------|
| Total Businesses             | 114,117                |
| Unique Categories              | 83,160                 |
| Cities Covered                 | 1,416                  |
| States                         | 22                     |
| 5-Star Businesses              | 43,488                 |
| Total Reviews Analyzed         | 150,346 (sampled from ~7M) |
| Overall Average Rating         | 3.75 stars             |

<img width="751" height="568" alt="image" src="https://github.com/user-attachments/assets/cd7ad63c-1fe4-4690-af93-4990b0e57712" />


## Key Insights & Dashboard Highlights

### 1. Business Distribution
<img width="1114" height="744" alt="image" src="https://github.com/user-attachments/assets/f0661759-5d86-4844-a5ee-2433c9dc2f81" />


### 2. Review & Sentiment Analysis
<img width="1114" height="794" alt="image" src="https://github.com/user-attachments/assets/37a40d21-1545-4e6a-90e0-761c9c015d0c" />


### Major Findings
- **93% Positive Reviews** (7% Negative, <1% Neutral)
- Positive reviews average **3.89 stars**, Negative only **2.01 stars**
- **Restaurants dominate** — Pizza and Mexican categories lead nationwide
- **Pennsylvania** has the highest business concentration (35K+ establishments)
- Review volume peaked in **2019 (907K reviews)** with sharp decline post-2020 (pandemic impact)


## Dashboard Features (Interactive in QuickSight)
- Filter by state, city, category, star rating, sentiment
- Top 5 genuine highest-rated restaurants per city
- Elite reviewer leaderboard
- Top 100 most useful/funny/cool reviews
- Review count vs average rating analysis
- Yearly and monthly trend exploration

## How to Run Locally / Reproduce
1. Download Yelp Academic Dataset from https://www.yelp.com/dataset
2. Run `python split_and_upload.py` → splits files & uploads to your S3 bucket
3. Execute Snowflake scripts in order
4. Connect QuickSight to Snowflake and import the provided dashboard templates


## Conclusion & Takeaways
<img width="809" height="667" alt="image" src="https://github.com/user-attachments/assets/e9fdd506-dec5-4ed7-9cfb-ee6444e557b3" />


This project is **fully replicates exactly what data teams at Yelp, Uber Eats, DoorDash, Zomato, etc. do daily** — just in a fully documented, portfolio-ready format.

**Perfect for Data Engineer, Data Analyst, or Business Intelligence Engineer roles.**

---
