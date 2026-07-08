## 상관계수 (Correlation Coefficient)

#### 피어슨 상관계수 (Pearson Correlation Coefficient)
두 변수 간의 선형적 연관성을 계량화한 수치입니다. 값의 범위는 $-1 \le r \le 1$ 입니다.

*   **모집단 상관계수 ($\rho$):**
    $$\rho_{X,Y} = \frac{\text{Cov}(X,Y)}{\sigma_X \sigma_Y}$$
*   **표본 상관계수 ($r$):**
    $$r = \frac{\sum (X_i - \bar{X})(Y_i - \bar{Y})}{\sqrt{\sum (X_i - \bar{X})^2 \sum (Y_i - \bar{Y})^2}}$$

#### 공분산 (Covariance)
두 변수가 함께 변하는 정도를 나타내는 지표입니다.
*   $$\text{Cov}(X,Y) = \frac{\sum (X_i - \bar{X})(Y_i - \bar{Y})}{n-1}$$

#### 스피어먼 순위 상관계수 (Spearman's Rank Correlation Coefficient)
두 변수의 순위 자료를 이용한 비모수적 상관분석 지표입니다. 데이터가 서열척도이거나 선형 관계를 따르지 않을 때 사용합니다.
*   $$\rho = 1 - \frac{6 \sum d_i^2}{n(n^2 - 1)}$$
    *   ($d_i$: 각 데이터의 두 변수 간 순위 차이, $n$: 데이터 개수)
