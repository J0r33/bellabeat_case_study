# Bellabeat Case Study: Smart Device Usage Insights
Using Fitbit public data to inform Bellabeat engagement and marketing  
**Author:** Joree Weatherly  
**Date:** 2025-11-03

---

## 1. Business Task (ASK)
**Objective:**  
Identify trends in smart device usage and recommend how Bellabeat can use those trends to improve user engagement and marketing.

**Key questions:**
1. What are some trends in smart device usage?
2. How could these trends apply to Bellabeat customers?
3. How could these trends help influence Bellabeat marketing strategy?

**Audience:** Bellabeat marketing/product stakeholders, portfolio reviewers.

---

## 2. Data (PREPARE)
**Source:** Public Fitbit Fitness Tracker Data (Kaggle)  
**Period:** March–May 2016  
**Users:** ~30 device owners  
**Tables used:**
- dailyActivity
- hourlyCalories
- hourlyIntensities
- hourlySteps
- minute-level sleep (aggregated to nightly)

**Note:** dataset is directional, not representative of actual Bellabeat users.

---

## 3. Limitations
- Non-Bellabeat users → behavior may differ from target women’s wellness segment
- Small + uneven sample (not all users track sleep/activity consistently)
- Short time window (~2 months)
- Consumer-grade device accuracy
- No demographics → no segmentation

**Implication:** insights are **exploratory** → best used to shape hypotheses and engagement ideas.

---

## 4. Tools & Processing (PROCESS)
**R packages:**
- `tidyverse` for wrangling/plots
- `janitor` to clean column names
- `lubridate` to parse dates/times
- `skimr` to profile data

**Key steps:**
1. Import A→M and M→A CSVs
2. Clean column names
3. Standardize datetime (`mdy()`, `mdy_hms()`)
4. Validate counts and date ranges
5. Merge into unified daily + hourly tables
6. Join hourly steps + calories + intensities
7. Create hour/day/weekday features

Result: tidy, analysis-ready tables for time-of-day and behavior-pattern analysis.

---

## 5. Analysis Questions (ANALYZE)
1. What hours of the day show highest activity?
2. How does weekday activity differ from weekend activity?
3. What is the relationship between intensity and calories?
4. Are steps a good proxy for intensity/engagement?
5. How many users meet the 10,000-step goal?
6. What proportion of waking time is sedentary?
7. Does total active distance relate to calories burned?

---

## 6. Finding #1 – Activity Peaks by Time of Day
**Observation:** Users are most active between ~10:00 and 19:00 (UTC); activity drops sharply overnight.

**Interpretation:** People have a daytime movement rhythm with morning and late-afternoon peaks.

**What Bellabeat can do:**
- Schedule push notifications during natural activity windows
- Send evening wind-down / mindfulness content after peak movement

---

## 7. Finding #2 – Weekday vs Weekend
**Observation:**  
- Weekdays start earlier; activity tied to workday rhythm  
- Weekends start later but can reach similar peaks

**What Bellabeat can do:**
- Weekdays → short, practical “movement break” nudges
- Weekends → longer, flexible wellness/challenge content

---

## 8. Finding #3 – Intensity ↔ Calories
**Observation:** Higher total intensity is associated with higher calories burned. Even moderate increases help.

**What Bellabeat can do:**
- Turn intensity gains into motivational messages (“You burned more today because you moved more intensely”)
- Educate that small increases in effort matter

---

## 9. Finding #4 – Steps ↔ Intensity
**Observation:** More steps per hour → higher average intensity. Steps work as a simple proxy for engagement.

**What Bellabeat can do:**
- Emphasize step-based goals and streaks (low friction, easy to understand)
- Position steps as “everyday activity” rather than workouts

---

## 10. Finding #5 – Most Days < 10,000 Steps
**Observation:**  
- Avg ≈ 7,200 steps/day  
- Only ~30% of days reach 10,000 steps

**What Bellabeat can do:**
- Use adaptive / incremental goals (“add 1,000 steps today”)
- Celebrate progress over perfection to prevent drop-off

---

## 11. Finding #6 – Sedentary vs Active Time
**Observation:** After adjusting for sleep, users spend ~2/3 of their waking time sedentary.

**What Bellabeat can do:**
- Promote “micro-activity” and hourly move reminders
- Show daily active-time rings/visuals to make sitting visible
- Frame wellness as small, frequent movement

---

## 12. Strategic Recommendations (SHARE / ACT)
1. **Timing:** send messages when users are already active (late morning, mid-afternoon).
2. **Personalized goals:** set realistic, incremental step targets for users below 10k.
3. **Micro-movement:** introduce short challenges to reduce sedentary time.
4. **Motivational framing:** “total movement matters” → light/moderate activity still counts.
5. **Next step for Bellabeat:** run the same pipeline on first-party Bellabeat data to segment by user type.

---

## 13. Conclusion
- Real-world wearable data shows moderate, everyday movement is the norm.
- Bellabeat can win by **supporting attainable wellness**, not only high-intensity fitness.
- Turning usage patterns into **well-timed, personalized nudges** is the fastest path to higher engagement.

---

## 14. Repo Notes
This presentation summarizes the analysis contained in:
- R Markdown analysis script (`bellabeat_case_study.Rmd`)
- Data cleaning, merging, and time-based feature engineering steps
- Insight → action mapping for Bellabeat
