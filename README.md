# coffee-heartdisease-stats
[![Kaggle](https://img.shields.io/badge/Kaggle-Notebook-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/code/paredes32/coffee-and-heartdisease))
[![GitHub](https://img.shields.io/badge/GitHub-Code-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/paredes32/coffee-heartdisease)

## 주요 분석 결과
| 항목                        | 결과                     | 통계적 유의성                |
|-----------------------------|--------------------------|------------------------------|
| 커피 섭취 ↔ 심장병 위험      | r = 0.30                 | Pearson, **p < 0.001**       |
| 연령 → 심장병 위험           | r ≈ 0.60                 | Pearson, **p < 0.001**       |
| 운동 없음 vs 자주 운동       | –0.85 (위험도 감소)      | Tukey HSD, **p < 0.001**     |
| 운동 없음 vs 가끔 운동       | –0.33                    | Tukey HSD, p = 0.146         |
| 가끔 운동 vs 자주 운동       | –0.52                    | Tukey HSD, **p = 0.014**      |
---
## 사용 기술
- Python, NumPy, Matplotlib, SciPy, Pandas, Statsmodels
- Pearson correlation, One-way ANOVA, Tukey HSD post-hoc test

## 시각화
<p align="center">
  <img src="scatter-plot.png" width="800"><br><br>
  <img src="causality-graph.png" width="850">
</p>
