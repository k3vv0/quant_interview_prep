# quant_interview_prep
Popular quant interview questions in probability, statistics, and data science.

## Formulas
### Combinatorics
- **Factorial**: $$n! = n * (n-1) * (n-2) * ... * 1$$
- **Permutations**: $$P(n, k) = \frac{n!}{(n-k)!}$$
- **Combinations**: $$C(n, k) = \frac{n!}{k! * (n-k)!}$$
- **Binomial Coefficient**: $$C(n, k) = \frac{n!}{k! * (n-k)!}$$
- **Binomial Theorem**: $$(x + y)^n = \sum_{k=0}^{n} C(n, k) * x^{n-k} * y^k$$
- **Multinomial Coefficient**: $$C(n, k_1, k_2, ..., k_m) = \frac{n!}{k_1! * k_2! * ... * k_m!}$$
- **Multinomial Theorem**: $$(x_1 + x_2 + ... + x_m)^n = \sum_{k_1 + k_2 + ... + k_m = n} C(n, k_1, k_2, ..., k_m) * x_1^{k_1} * x_2^{k_2} * ... * x_m^{k_m}$$
- **Stars and Bars with Indestinguishable Objects**: $$C(n+k-1, k-1)$$
- **Stars and Bars with Distinct Objects**: $$C(n-1, k-1)$$

### Probability
- **Bayes' Theorem**: $$P(A|B) = \frac{P(B|A) * P(A)}{P(B)}$$
- **Conditional Probability**: $$P(A|B) = \frac{P(A \cap B)}{P(B)}$$
- **Total Probability**: $$P(A) = P(A|B_1) * P(B_1) + P(A|B_2) * P(B_2) + ... + P(A|B_n) * P(B_n)$$
- **Law of Total Expectation**: $$E(X) = E(E(X|Y))$$
- **Law of Total Variance**: $$Var(X) = E(Var(X|Y)) + Var(E(X|Y))$$
- **Law of Total Covariance**: $$Cov(X, Y) = E(Cov(X, Y|Z)) + Cov(E(X|Z), E(Y|Z))$$
- **Law of Total Correlation**: $$Corr(X, Y) = E(Corr(X, Y|Z)) + Corr(E(X|Z), E(Y|Z))$$
- **Law of Total Conditional Expectation**: $$E(X|Y) = E(E(X|Y, Z))$$
- **Law of Total Conditional Variance**: $$Var(X|Y) = E(Var(X|Y, Z)) + Var(E(X|Y, Z))$$
- **Law of Total Conditional Covariance**: $$Cov(X, Y|Z) = E(Cov(X, Y|Y, Z)) + Cov(E(X|Y, Z), E(Y|Y, Z))$$
- **Law of Total Conditional Correlation**: $$Corr(X, Y|Z) = E(Corr(X, Y|Y, Z)) + Corr(E(X|Y, Z), E(Y|Y, Z))$$
### Statistics
- **Mean**: $$\mu = \frac{\sum_{i=1}^{n} x_i}{n}$$
- **Variance**: $$\sigma^2 = \frac{\sum_{i=1}^{n} (x_i - \mu)^2}{n}$$
- **Standard Deviation**: $$\sigma = \sqrt{\sigma^2}$$
- **Covariance**: $$Cov(X, Y) = \frac{\sum_{i=1}^{n} (x_i - \mu_x) * (y_i - \mu_y)}{n}$$
- **Correlation**: $$Corr(X, Y) = \frac{Cov(X, Y)}{\sigma_x * \sigma_y}$$
- **Least Squares Regression Line**: $$y = mx + b$$
- **Least Squares Regression Slope**: $$m = \frac{\sum_{i=1}^{n} (x_i - \mu_x) * (y_i - \mu_y)}{\sum_{i=1}^{n} (x_i - \mu_x)^2}$$
- **Least Squares Regression Intercept**: $$b = \mu_y - m * \mu_x$$
- **Least Squares Regression Line Prediction**: $$\hat{y} = m * x + b$$
- **Least Squares Regression Line Residual**: $$e = y - \hat{y}$$
- **Least Squares Regression Line Residual Sum of Squares**: $$RSS = \sum_{i=1}^{n} e_i^2$$
- **Least Squares Regression Line Total Sum of Squares**: $$TSS = \sum_{i=1}^{n} (y_i - \mu_y)^2$$
- **Least Squares Regression Line Explained Sum of Squares**: $$ESS = \sum_{i=1}^{n} (\hat{y_i} - \mu_y)^2$$
- **Least Squares Regression Line R-Squared**: $$R^2 = \frac{ESS}{TSS} = 1 - \frac{RSS}{TSS}$$
- **Least Squares Regression Line Standard Error**: $$SE = \sqrt{\frac{RSS}{n-2}}$$
- **Least Squares Regression Line Confidence Interval**: $$CI = m \pm t_{\alpha/2} * SE$$
- **Least Squares Regression Line Prediction Interval**: $$PI = \hat{y} \pm t_{\alpha/2} * SE$$
- **Least Squares Regression Line Hypothesis Test**: $$t = \frac{m - 0}{SE}$$
- **Least Squares Regression Line Hypothesis Test P-Value**: $$P = 2 * (1 - t_{n-2})$$
- **Least Squares Regression Line Hypothesis Test Confidence Interval**: $$CI = m \pm t_{n-2} * SE$$
- **Least Squares Regression Line Hypothesis Test Prediction Interval**: $$PI = \hat{y} \pm t_{n-2} * SE$$
- **Least Squares Regression Line Hypothesis Test F-Statistic**: $$F = \frac{ESS/k}{RSS/(n-k-1)}$$
- **Least Squares Regression Line Hypothesis Test F-Statistic P-Value**: $$P = 1 - F_{n-k-1, k}$$
- **Least Squares Regression Line Hypothesis Test F-Statistic Confidence Interval**: $$CI = \frac{1}{F_{k, n-k-1}}$$
- **Least Squares Regression Line Hypothesis Test F-Statistic Prediction Interval**: $$PI = \frac{1}{F_{k, n-k-1}}$$
- **Least Squares Regression Line Hypothesis Test Chi-Squared Statistic**: $$\chi^2 = \frac{n * R^2}{1 - R^2}$$
- **Least Squares Regression Line Hypothesis Test Chi-Squared Statistic P-Value**: $$P = 1 - \chi^2_{1, n-2}$$
- **Least Squares Regression Line Hypothesis Test Chi-Squared Statistic Confidence Interval**: $$CI = \frac{1}{\chi^2_{n-2, 1}}$$
- **Least Squares Regression Line Hypothesis Test Chi-Squared Statistic Prediction Interval**: $$PI = \frac{1}{\chi^2_{n-2, 1}}$$
- **Least Squares Regression Line Hypothesis Test Z-Statistic**: $$Z = \frac{m - 0}{SE}$$
- **Least Squares Regression Line Hypothesis Test Z-Statistic P-Value**: $$P = 2 * (1 - Z)$$
- **Least Squares Regression Line Hypothesis Test Z-Statistic Confidence Interval**: $$CI = m \pm Z$$
- **Least Squares Regression Line Hypothesis Test Z-Statistic Prediction Interval**: $$PI = \hat{y} \pm Z$$
- **Least Squares Regression Line Hypothesis Test T-Statistic**: $$T = \frac{m - 0}{SE}$$
- **Least Squares Regression Line Hypothesis Test T-Statistic P-Value**: $$P = 2 * (1 - T_{n-2})$$
- **Least Squares Regression Line Hypothesis Test T-Statistic Confidence Interval**: $$CI = m \pm T_{n-2} * SE$$
- **Least Squares Regression Line Hypothesis Test T-Statistic Prediction Interval**: $$PI = \hat{y} \pm T_{n-2} * SE$$
