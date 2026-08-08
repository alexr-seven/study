# Study Topics for Claude

**Purpose:** Interview prep for ML/AI roles and ML-for-quant-finance roles (hedge funds).
**How to use:** Give Claude the raw GitHub URL at the start of a session, then say
e.g. "Open my study topics doc, let's go through Stochastic Calculus." Use the seed
prompt style: state your background, ask for derivations not just definitions, and
end with self-check questions. Mark items `[x]` as you cover them; keep a running
note under each item for gaps to revisit.

---

## 1. Linear Algebra Fundamentals
- [ ] Vector spaces, basis, rank, null space
- [ ] Eigenvalues/eigenvectors, diagonalization, spectral theorem
- [ ] SVD — derivation, geometric interpretation, relation to PCA
- [ ] Positive definite/semidefinite matrices
- [ ] Matrix calculus (gradients, Jacobians, Hessians) for ML derivations
- [ ] Norms, condition number, numerical stability

## 2. Calculus & Optimization Fundamentals
- [ ] Multivariate calculus, chain rule, Taylor expansion
- [ ] Convexity, convex sets/functions, first/second-order conditions
- [ ] Lagrangian duality, KKT conditions
- [ ] Gradient descent, SGD, momentum, Adam — derivations and failure modes
- [ ] Second-order methods (Newton, quasi-Newton) — trade-offs
- [ ] Constrained optimization in ML (e.g. SVM dual)

## 3. Probability
- [ ] Axioms, conditional probability, Bayes' theorem
- [ ] Random variables, distributions (discrete/continuous), moment generating functions
- [ ] Law of large numbers, central limit theorem
- [ ] Measure-theoretic probability (in progress — Rosenthal → Durrett path)
- [ ] Convergence types: a.s., in probability, in distribution, in L^p
- [ ] Martingales — definitions, optional stopping, applications

## 4. Statistics
- [ ] Estimation theory: MLE, MAP, method of moments
- [ ] Bias, variance, consistency, efficiency, sufficiency
- [ ] Hypothesis testing, p-values, power, multiple testing correction
- [ ] Confidence intervals vs credible intervals
- [ ] Bayesian statistics: priors, posteriors, conjugacy, MCMC basics
- [ ] Resampling: bootstrap, permutation tests
- [ ] Asymptotic theory (CLT variants, delta method)

## 5. Information Theory
- [ ] Entropy, cross-entropy, KL divergence, mutual information
- [ ] Relation to log-likelihood and loss functions in ML
- [ ] Channel capacity, coding theory basics (light touch)
- [ ] MDL / information-theoretic model selection

## 6. Statistical Learning Theory
- [ ] Bias-variance tradeoff — formal decomposition
- [ ] VC dimension, PAC learning, generalization bounds
- [ ] Rademacher complexity
- [ ] Regularization as inductive bias (L1/L2, early stopping)
- [ ] No free lunch theorem

## 7. Machine Learning (Classical)
- [ ] Linear/logistic regression — derivations, assumptions, diagnostics
- [ ] Regularization: ridge, lasso, elastic net — derive closed forms
- [ ] Tree-based methods: decision trees, random forests, gradient boosting (derive GBM)
- [ ] SVMs — margin, kernel trick, dual formulation
- [ ] Naive Bayes, k-NN
- [ ] Clustering: k-means, hierarchical, DBSCAN, GMMs + EM algorithm
- [ ] Dimensionality reduction: PCA, t-SNE, UMAP (intuition)
- [ ] Model evaluation: cross-validation, ROC/AUC, calibration
- [ ] Feature engineering, feature selection

## 8. Deep Learning
- [ ] Backpropagation — derive from scratch
- [ ] Activation functions, vanishing/exploding gradients
- [ ] CNNs — convolution math, receptive fields, pooling
- [ ] RNNs/LSTMs/GRUs — gating derivations, why they help with gradients
- [ ] Attention & Transformers — derive self-attention, positional encoding
- [ ] Normalization: batchnorm, layernorm — why they work
- [ ] Optimization in DL: learning rate schedules, warmup, weight decay
- [ ] Regularization in DL: dropout, data augmentation, label smoothing
- [ ] Generative models: autoencoders, VAEs, GANs, diffusion models (intuition + math)

## 9. NLP & LLMs
- [ ] Tokenization, embeddings, word2vec/GloVe intuition
- [ ] Transformer architecture end-to-end
- [ ] Pretraining objectives (causal LM, masked LM)
- [ ] Fine-tuning, RLHF/DPO basics
- [ ] Scaling laws
- [ ] Evaluation of LLMs, hallucination, retrieval-augmented generation

## 10. Time Series
- [ ] Stationarity, autocorrelation, unit roots
- [ ] ARIMA / SARIMA — derive, identify orders
- [ ] State space models, Kalman filter — derive
- [ ] Volatility models: ARCH/GARCH
- [ ] Cointegration, error correction models
- [ ] Forecasting evaluation, backtesting pitfalls (lookahead bias)
- [ ] Deep learning for time series (temporal CNNs, transformers for sequences)

## 11. Econometrics
- [ ] OLS assumptions, Gauss-Markov theorem
- [ ] Endogeneity, omitted variable bias, measurement error
- [ ] Instrumental variables, 2SLS
- [ ] Panel data: fixed effects, random effects
- [ ] Heteroskedasticity, autocorrelation, robust standard errors
- [ ] GMM estimation

## 12. Causal Inference
- [ ] Potential outcomes framework, ATE/ATT
- [ ] Randomized experiments vs observational data
- [ ] Confounding, DAGs, backdoor criterion
- [ ] Propensity score matching/weighting
- [ ] Difference-in-differences
- [ ] Regression discontinuity
- [ ] Instrumental variables (causal framing)
- [ ] Synthetic control

## 13. Quant Finance — Derivatives & Stochastic Calculus
- [ ] Financial derivatives fundamentals: forwards, futures, options, swaps
- [ ] Put-call parity, arbitrage-free pricing
- [ ] Brownian motion, Itô's lemma — derive
- [ ] Risk-neutral valuation, martingale pricing
- [ ] Black-Scholes — derive PDE and closed-form solution
- [ ] Greeks — derive and interpret
- [ ] Volatility surface, implied vol, local/stochastic vol models
- [ ] Interest rate models (brief): Vasicek, CIR

## 14. Quant Finance — Portfolio & Risk
- [ ] Mean-variance optimization, efficient frontier
- [ ] CAPM, Fama-French factor models
- [ ] Sharpe ratio, Sortino, other risk-adjusted metrics
- [ ] VaR, CVaR/expected shortfall
- [ ] Risk parity, factor investing
- [ ] Backtesting methodology, overfitting in strategy design

## 15. Quant Finance — Market Microstructure & Systematic Trading
- [ ] Order book dynamics, bid-ask spread, market impact
- [ ] Execution algorithms (TWAP/VWAP, implementation shortfall)
- [ ] Alpha signal construction and decay
- [ ] Statistical arbitrage / pairs trading (cointegration link back to §10-11)
- [ ] High-frequency vs low-frequency strategy considerations

## 16. Python & Algorithms
- [ ] Core data structures: arrays, hash maps, trees, heaps, graphs
- [ ] Algorithmic complexity, common patterns (two pointers, sliding window, DP)
- [ ] Sorting/searching, graph algorithms (BFS/DFS, shortest path)
- [ ] Python for ML: numpy/pandas idioms, vectorization
- [ ] Writing efficient, correct code under interview time pressure

## 17. Experimentation & A/B Testing
- [ ] Designing experiments, power analysis
- [ ] Common pitfalls: peeking, novelty effects, network effects
- [ ] Sequential testing, multi-armed bandits

## 18. ML Systems / MLOps (light touch — flag relevance per interview)
- [ ] Training/serving pipelines, feature stores
- [ ] Model monitoring, drift detection
- [ ] Scalability considerations (batch vs online inference)

---

## Gaps Log
*(Running list of things to revisit — add after each session)*
-

## Session Notes
*(Optional: date + topic + key takeaway)*
-
