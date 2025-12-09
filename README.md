# Coffee-HeartDisease-Stats

Analysis of simulated data exploring the relationship between coffee consumption, age, exercise, and heart disease risk. This project uses Python to generate data, compute correlations, visualize relationships, and perform statistical tests like ANOVA with post-hoc analysis.

## Project Overview
This Jupyter notebook simulates 1000 data points to investigate potential confounders (e.g., age) in the coffee-heart disease link. It includes scatter plots, Pearson correlations, and multi-group comparisons via Tukey HSD to assess exercise's impact.

## 주요 분석 결과

| 항목                  | 결과                          | 통계적 유의성                  |
|-----------------------|-------------------------------|--------------------------------|
| 커피 소비 vs 심장병 위험 | 상관계수: 0.30               | Pearson r, p < 0.001           |
| 연령 vs 심장병 위험     | 상관계수: 0.60 (추정)        | Pearson r, p < 0.001           |
| 운동なし vs 자주 운동  | 평균 차이: -0.85             | Tukey HSD, p < 0.001           |
| 운동なし vs 가끔 운동  | 평균 차이: -0.33             | Tukey HSD, p = 0.146 (유의X)   |
| 가끔 운동 vs 자주 운동 | 평균 차이: -0.52             | Tukey HSD, p = 0.014           |

- **해석**: 커피 소비와 심장병 위험 간 약한 양의 상관이 있지만, 연령이 confounding factor일 수 있음. 운동 증가 시 심장병 위험이 유의하게 감소.

## 사용 기술
* Python, NumPy, Matplotlib, SciPy, Pandas, Statsmodels
* Pearson 상관분석, ANOVA, Tukey HSD 사후 분석

## How to Run
1. Clone the repo: `git clone https://github.com/paredes32/coffee-heartdisease-stats.git`
2. Install dependencies: `pip install numpy matplotlib scipy pandas statsmodels`
3. Open the notebook: `jupyter notebook coffee-and-heartdisease.ipynb`
4. Run all cells to reproduce results.

## Visualizations
![Coffee vs Heart Disease Scatter Plot](scatter-plot.png)  
Correlation coefficient between coffee consumption and risk of heart disease: 0.65

## Limitations
- Data is simulated (random normal distribution); real-world data may differ.
- Assumes linear relationships; further modeling (e.g., regression) recommended.

For questions, open an issue or contact me!
