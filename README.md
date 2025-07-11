# AI_assistant_usage_student_life
📘 Project Title:
Exploratory Data Analysis and Statistical Testing on AI Assistant Usage in Student Life

🧾 Dataset Overview:
This dataset captures information about how students from various academic levels and disciplines interact with AI assistants for different academic tasks, and how that correlates with session lengths, prompt counts, satisfaction levels, and whether they'd use it again.

📂 File: ai_assistant_usage_student_life.csv
📊 Rows: ~15,000+
🔢 Columns: 13 features, including categorical, continuous, and date-derived variables.

### 🔢 Features Description

| Column               | Type         | Description |
|----------------------|--------------|-------------|
| `StudentLevel`       | Categorical  | Education level (e.g., High School, Undergraduate, Graduate) |
| `Discipline`         | Categorical  | Field of study (e.g., CS, Business, Math) |
| `SessionLengthMin`   | Continuous   | Total duration of AI assistant session in minutes |
| `TotalPrompts`       | Continuous   | Number of prompts sent to the assistant |
| `TaskType`           | Categorical  | Type of academic task (e.g., Coding, Studying) |
| `AI_AssistanceLevel` | Ordinal      | Level of AI guidance requested (1 to 5) |
| `FinalOutcome`       | Categorical  | Result of the session (e.g., Completed, Gave Up) |
| `UsedAgain`          | Binary       | Whether the student would use the AI again (0 = Yes, 1 = No) |
| `SatisfactionRating` | Continuous   | Student satisfaction rating (1.0 to 5.0) |
| `S_Year`             | Categorical  | Year of session (2024, 2025) |
| `S_Month`            | Categorical  | Month of session (1–12) |
| `S_Day`              | Categorical  | Day of the month (1–31) |
| `S_Week`             | Categorical  | Week number of the year (1–52) |

---

### 🔬 Statistical Tests Applied

| Test Type           | Condition                              | Purpose |
|---------------------|----------------------------------------|---------|
| **Two-sample t-test**     | Continuous vs Continuous                | Tests if two numeric columns have different means |
| **ANOVA**           | Continuous vs Categorical              | Tests if a numeric feature varies significantly across groups |
| **Chi-squared test**| Categorical vs Categorical             | Tests association between two categorical variables |

---

### 🔧 Feature Encoding Strategy

| Encoding Method     | Used For                              |
|---------------------|----------------------------------------|
| **OrdinalEncoder**  | Features with natural order (e.g., `StudentLevel`, `AI_AssistanceLevel`) |
| **No Encoding**     | For numerical and datetime features unless required |
