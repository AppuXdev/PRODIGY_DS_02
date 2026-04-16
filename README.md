# Task 2: Titanic Dataset - EDA & Data Cleaning

## Dataset
- **Source**: Prodigy-InfoTech Task 2 Dataset
- **Link**: https://github.com/Prodigy-InfoTech/data-science-datasets/tree/main/Task%202
- **File**: train.csv
- **Records**: 891 rows, 12 columns
- **Columns**: PassengerId, Survived, Pclass, Name, Sex, Age, SibSp, Parch, Ticket, Fare, Cabin, Embarked

## Objective
Perform data cleaning and exploratory data analysis on train.csv to explore relationships between variables and identify patterns in passenger survival data.

## Files
- `gtrain.ipynb` - Jupyter notebook with complete EDA and visualizations
- `train.py` - Python script version of the analysis
- `train.csv` - Training dataset with 891 passenger records

## Analysis Performed

### 1. Data Cleaning
- **Age**: 177 missing values filled with median 28.0
- **Embarked**: 2 missing values filled with mode 'S'
- **Cabin**: Dropped column due to 77% missing values
- **Feature Engineering**: Created `FamilySize` and `IsAlone` features

### 2. Univariate Analysis
- Overall survival rate: 38.38%
- Distribution of passenger class, age, gender

### 3. Bivariate Analysis
- **Survival vs Sex**: Females 74.2% vs Males 18.9%
- **Survival vs Pclass**: 1st class 63.0% vs 3rd class 24.2%
- **Survival vs Age**: Children <10 had higher survival rates

### 4. Multivariate Analysis
- Correlation heatmap of numeric features
- Strong negative correlation: Pclass vs Survival (-0.34)
- Positive correlation: Fare vs Survival (0.26)

## Key Insights
1. **Gender** was the strongest predictor - "Women and children first" policy evident
2. **Socioeconomic status** mattered - 1st class passengers had 2.6x better odds than 3rd class
3. **Age** influenced survival - children prioritized, ages 20-40 had lowest rates
4. **Family size** had impact - passengers alone had lower survival than small families
5. **Fare** correlates with survival as proxy for class

## Tech Stack
`Python` `Pandas` `NumPy` `Matplotlib` `Seaborn` `Jupyter Notebook`

## How to Run
1. Clone repository
2. Install dependencies: `pip install pandas matplotlib seaborn jupyter`
3. **
4. 
