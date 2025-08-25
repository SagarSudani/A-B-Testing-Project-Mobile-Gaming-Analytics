🎮 **A/B Testing in Mobile Gaming – Cookie Cats Dataset**
📌 Project Overview

This project analyzes player behavior in a mobile puzzle game (Cookie Cats) to evaluate how tutorial gate placement affects player engagement and retention.
Using A/B testing and statistical hypothesis testing, we compare two groups of players:

gate_30 → tutorial gate at level 30 (Control group)

gate_40 → tutorial gate at level 40 (Treatment group)

The analysis includes:

Descriptive statistics of player engagement (game rounds played).

T-tests for comparing average playtime between groups.

Chi-square tests for comparing retention rates (Day-1 and Day-7).

Practical insights into game design and player retention strategies.

📂 Dataset

The dataset cookie_cats.csv contains ~90,000 player records with the following key columns:

userid → Unique player ID

version → Experiment group (gate_30 / gate_40)

sum_gamerounds → Total number of rounds played by the player

retention_1 → Whether the player returned 1 day after install (0/1)

retention_7 → Whether the player returned 7 days after install (0/1)

⚙️ Technologies Used

Python 🐍

Pandas → Data cleaning & manipulation

SciPy → Statistical tests (t-test, chi-square)

Matplotlib / Seaborn → Data visualization

📊 Analysis Workflow

Load & Explore Data → Inspect dataset and split groups (gate_30 vs gate_40).

Engagement Analysis → Compare average game rounds using a t-test.

Retention Analysis → Compare Day-1 & Day-7 retention rates using a chi-square test.

Interpret Results → Translate statistical results (p-values, effect sizes) into business insights.

🚀 How to Run

Clone this repository:

git clone https://github.com/yourusername/ab-testing-cookie-cats.git
cd ab-testing-cookie-cats


Install required libraries:

pip install pandas scipy matplotlib seaborn


Run the analysis:

python ab_test_analysis.py

📈 Key Findings

Game Rounds: No significant difference in average playtime between groups.

Day-1 Retention: Slight difference, but not statistically significant.

Day-7 Retention: Statistically significant difference — players with gate at level 30 retained better.

👉 Recommendation: Keep the tutorial gate at level 30 to maximize long-term player retention.

🔑 Learning Outcomes

Practical application of A/B testing on real game data.

Hands-on experience with hypothesis testing (t-test & chi-square).

Data-driven approach to player engagement & retention analysis.
