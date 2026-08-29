# 🔴 ShadowFox Data Science Internship – Advanced Task

## Cricket Fielding Analysis Data Collection

This project is part of the **ShadowFox Data Science Internship – Advanced Level**.

The task focuses on collecting and analyzing fielding performance data for three selected players from a T20 cricket match. The objective is to evaluate individual fielding contributions and understand their impact on the team's defensive performance.

---

## 📌 Task Objective

As a sports analyst with an interest in cricket, the objective is to conduct a detailed fielding performance analysis for three players from a T20 match.

The collected data is used to:

- Record fielding actions for each ball
- Measure individual fielding contributions
- Identify strengths and weaknesses
- Calculate a Performance Score
- Compare the selected players
- Identify areas for fielding improvement
- Support strategic fielding decisions

---

## 🏏 Match and Players

The sample analysis is based on:

**Match:** ICC Men's T20 World Cup 2024 Final – India vs South Africa

**Innings Analyzed:** 2nd Innings  
**Team Fielding:** India  
**Venue:** Kensington Oval, Bridgetown, Barbados

### Players Analyzed

1. Suryakumar Yadav
2. Ravindra Jadeja
3. Axar Patel

The analysis covers the fielding involvement of these three players during the innings.

---

## 📊 Dataset Features

The fielding dataset contains the following features:

| Feature | Description |
|---|---|
| Match No. | Identifier for the match |
| Innings | Innings in which the fielding data is recorded |
| Team | Team currently fielding |
| Player Name | Fielder involved in the action |
| BallCount | Sequence number of the ball |
| Position | Fielding position |
| Short Description | Description of the fielding event |
| Pick | Category of the fielding action |
| Throw | Category of the throwing action |
| Runs | Runs saved or conceded through the fielding effort |
| Overcount | Over in which the event occurred |
| Venue | Match location |

---

## 🧾 Fielding Action Codes

### Pick Codes

| Code | Meaning |
|---|---|
| Y | Clean Pick |
| N | Fumble |
| C | Catch |
| DC | Dropped Catch |
| S | Stumping |

### Throw Codes

| Code | Meaning |
|---|---|
| Y | Good Throw |
| N | Bad Throw |
| DH | Direct Hit |
| RO | Run Out |
| MR | Missed Run Out |

### Runs

The `Runs` field represents the impact of the fielding effort:

- Positive value (+) → Runs saved
- Negative value (-) → Runs conceded

---

## 🧮 Performance Score

The fielding performance is evaluated using the following formula:

```text
PS = (CP × W_CP)
   + (GT × W_GT)
   + (C × W_C)
   − (DC × W_DC)
   + (ST × W_ST)
   + (RO × W_RO)
   − (MRO × W_MRO)
   + (DH × W_DH)
   + RS

---

## 🔍 Data Collection Process

For each ball bowled in the selected innings, the fielding effort is recorded according to the defined dataset features.

The process includes:

Identify the ball and over.
Identify the fielder involved.
Record the fielding position.
Describe the fielding event.
Record the Pick category.
Record the Throw category.
Record runs saved or conceded.
Store the venue and match information.
Repeat the process for the complete innings.

📈 Performance Analysis

The collected fielding data is aggregated for the three selected players.
The sample Performance Matrix gives the following results:
| Player           | Clean Picks | Good Throws | Catches | Dropped Catches | Stumpings | Run Outs | Missed Run Outs | Direct Hits | Runs Saved | Performance Score |
| ---------------- | ----------: | ----------: | ------: | --------------: | --------: | -------: | --------------: | ----------: | ---------: | ----------------: |
| Suryakumar Yadav |           5 |           5 |       1 |               1 |         0 |        0 |               0 |           0 |          1 |                11 |
| Ravindra Jadeja  |           8 |           5 |       0 |               1 |         0 |        0 |               0 |           1 |          3 |                15 |
| Axar Patel       |           7 |           6 |       0 |               0 |         0 |        0 |               1 |           0 |          1 |                12 |


🏆 Key Findings

Suryakumar Yadav

Strength:
Produced a match-defining catch under pressure.
Recorded 5 clean picks and 5 good throws.
The catch contributes significantly to the Performance Score.

Area for Improvement:
Recorded one dropped catch.
Catching reliability under difficult/high-pressure situations can be improved.

Ravindra Jadeja

Strength:
Had the highest Performance Score in the sample: 15.
Recorded 8 clean picks.
Recorded 5 good throws.
Produced a direct hit.
Recorded 3 runs saved.

Area for Improvement:
Recorded a dropped catch.
Death-over catching under pressure can be a specific area for improvement.

Axar Patel

Strength:
Recorded 7 clean picks and 6 good throws.
Had no dropped catches in the sample.
Demonstrated reliable fielding during the middle overs.

Area for Improvement:
Recorded one missed run-out opportunity.
An early fumble indicates an opportunity to improve decision-making and handling under pace.

👥 Team-Level Analysis

All three players achieved positive Performance Scores despite recording some costly errors. The analysis demonstrates that consistent low-risk fielding actions such as clean picks and accurate throws can contribute significantly to overall fielding performance. The analysis highlights two main development priorities:
Catching reliability under pressure
Run-out decision-making in fast-moving situations

📊 Main Insight

The Performance Score provides a more meaningful measure of fielding impact than simply counting the number of fielding events.
High-impact actions such as catches, run-outs, and direct hits receive greater weights, while dropped catches and missed run-outs reduce the score.
Therefore, the scoring model helps distinguish between frequent routine actions and fewer but more influential fielding events.

🛠️ Tools Used
Microsoft Excel
Python
Pandas
NumPy
Matplotlib
Seaborn
Jupyter Notebook

📄 Deliverable

The ShadowFox Advanced Task requires a well-organized spreadsheet or database containing the complete fielding data for the selected match.
The project workbook contains:
Fielding data
Fielding action legend
Scoring weights
Performance Matrix
Performance Scores
Fielding analysis and insights

🎯 Learning Outcomes

Through this task, I developed practical experience in:
Cricket data analysis
Data collection
Data organization
Spreadsheet-based analysis
Performance metric calculation
Data interpretation
Identifying player strengths and weaknesses
Creating analytical insights
Applying a scoring model to real-world data

👨‍💻 Author

Vansh Srivastava
B.Tech – Computer Science and Engineering (CSE)
ShadowFox Data Science Intern

🏢 Internship

Organization: ShadowFox
Domain: Data Science
Level: Advanced
