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

## 2b. Differential Equations (light)
- [ ] First-order ODEs: separable, linear, integrating factors
- [ ] Systems of ODEs, equilibrium points, stability analysis
- [ ] Numerical methods: Euler, Runge-Kutta (intuition, not derivation-heavy)
- [ ] Connection to PDEs: heat equation, Black-Scholes PDE (link to §13)

## 2c. Fourier Analysis (light)
- [ ] Fourier series — intuition, orthogonal basis functions
- [ ] Fourier transform, convolution theorem
- [ ] Frequency-domain intuition for time series (spectral density)
- [ ] Connection to CNNs (convolution) and signal processing

## 2d. Real, Measure-Theoretic & Functional Analysis Foundations
- [ ] Sequences/series: convergence, Cauchy criterion, Bolzano-Weierstrass
- [ ] Compactness (Heine-Borel), continuity, uniform continuity
- [ ] Mean Value Theorem, Extreme Value Theorem
- [ ] Sigma-algebras, measures, Lebesgue measure — construction and intuition
- [ ] Measurable functions, random variables as measurable functions (link to §3)
- [ ] Lebesgue integration vs Riemann — why it matters, key differences
- [ ] Monotone convergence theorem, dominated convergence theorem, Fatou's lemma
- [ ] Fubini's theorem (light — when it applies)
- [ ] Functional analysis (light): normed/Banach spaces, Hilbert spaces, inner product spaces
- [ ] L^p spaces — intuition, relevance to statistics/ML
- [ ] RKHS (reproducing kernel Hilbert space) — light touch, ties to kernel methods (§7)

## 3. Probability
- [ ] Axioms, conditional probability, Bayes' theorem
- [ ] Random variables, distributions (discrete/continuous), moment generating functions
- [ ] Joint/marginal/conditional distributions, independence
- [ ] Covariance, correlation — properties and pitfalls
- [ ] Common distribution catalog and relationships (Binomial↔Poisson limit, sums of Bernoullis, memorylessness of Exponential/Geometric)
- [ ] Transformations of random variables: change of variables, order statistics, sums/convolution of RVs
- [ ] Conditional expectation — tower property, law of total variance
- [ ] Key inequalities: Markov, Chebyshev, Jensen, Cauchy-Schwarz, union bound
- [ ] Law of large numbers, central limit theorem
- [ ] Measure-theoretic probability foundations — see §2d; apply here (probability measures, expectation as Lebesgue integral)
- [ ] Convergence types: a.s., in probability, in distribution, in L^p
- [ ] Martingales — definitions, optional stopping, applications

## 3b. Combinatorics
- [ ] Counting principles: permutations, combinations
- [ ] Inclusion-exclusion principle
- [ ] Binomial/multinomial theorem, Pascal's triangle identities
- [ ] Generating functions (light)
- [ ] Applications to probability computations (birthday problem, etc.)

## 3c. Stochastic Processes & Markov Chains
- [ ] Markov chains: transition matrices, Chapman-Kolmogorov equations
- [ ] Stationary distributions, ergodicity, irreducibility, periodicity
- [ ] Absorbing states, absorption probabilities
- [ ] Random walks, gambler's ruin
- [ ] Poisson processes — memorylessness, interarrival times
- [ ] Monte Carlo simulation basics (link to §4b MCMC)

## 4. Statistics
- [ ] Estimation theory: MLE, MAP, method of moments
- [ ] Bias, variance, consistency, efficiency, sufficiency
- [ ] Hypothesis testing, p-values, power, multiple testing correction
- [ ] Confidence intervals vs credible intervals
- [ ] Resampling: bootstrap, permutation tests
- [ ] Asymptotic theory (CLT variants, delta method)

## 4b. Bayesian Statistics
- [ ] Bayes' theorem, prior/likelihood/posterior mechanics
- [ ] Conjugate priors — derive a few (Beta-Binomial, Normal-Normal)
- [ ] Point estimation: MAP vs posterior mean vs posterior median
- [ ] MCMC: Metropolis-Hastings, Gibbs sampling — intuition and derivation
- [ ] Variational inference (light — ELBO intuition)
- [ ] Bayesian model comparison, Bayes factors
- [ ] Hierarchical/multilevel models
- [ ] Bayesian vs frequentist — philosophical and practical trade-offs

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
- [ ] Regularization: ridge, lasso, elastic net — derive closed forms, geometric intuition
- [ ] Bias-variance in practice: learning curves, diagnosing under/overfitting
- [ ] Tree-based methods: decision trees (splitting criteria, Gini/entropy), random forests (bagging, feature subsampling)
- [ ] Gradient boosting — derive from functional gradient descent; XGBoost/LightGBM specifics (regularization terms, histogram binning, leaf-wise vs level-wise growth)
- [ ] Bagging vs boosting — bias-variance framing of why each works
- [ ] SVMs — margin, kernel trick (Mercer's theorem intuition), dual formulation, soft margin
- [ ] Kernel methods more broadly — RBF, polynomial, kernel ridge regression
- [ ] Naive Bayes, k-NN — assumptions, curse of dimensionality for k-NN
- [ ] Clustering: k-means (derive Lloyd's algorithm, convergence), hierarchical, DBSCAN, GMMs + EM algorithm (derive E-step/M-step)
- [ ] Dimensionality reduction: PCA (derive via eigendecomposition and via SVD), t-SNE, UMAP (intuition, when each is appropriate)
- [ ] Model evaluation: cross-validation (k-fold, stratified, time-series-aware), ROC/AUC, precision-recall trade-offs, calibration (Platt scaling, isotonic regression)
- [ ] Imbalanced classification: resampling (SMOTE), class weighting, threshold tuning, appropriate metrics
- [ ] Feature engineering, feature selection (filter/wrapper/embedded methods)
- [ ] Hyperparameter tuning: grid/random search, Bayesian optimization intuition
- [ ] Semi-supervised and self-training approaches (light)
- [ ] Anomaly/outlier detection: isolation forests, one-class SVM, statistical approaches

## 7b. Model Interpretability
- [ ] Partial dependence plots (PDPs) — construction, limitations (correlated features)
- [ ] Individual conditional expectation (ICE) plots
- [ ] SHAP — Shapley values derivation, additive feature attribution, TreeSHAP vs KernelSHAP
- [ ] LIME — local surrogate models, how it differs from SHAP
- [ ] Permutation feature importance vs impurity-based importance
- [ ] Global vs local interpretability — when each is appropriate
- [ ] Interpretability-accuracy trade-offs, regulatory context (credit, healthcare)

## 8. Deep Learning
- [ ] Backpropagation — derive from scratch, computational graph view
- [ ] Weight initialization: Xavier/Glorot, He initialization — derive why they matter
- [ ] Activation functions, vanishing/exploding gradients — mechanisms and fixes
- [ ] Loss functions: cross-entropy derivation, focal loss, contrastive/triplet losses
- [ ] Loss landscape intuition: saddle points vs local minima in high dimensions
- [ ] CNNs — convolution math, receptive fields, pooling, ResNets (skip connections — why they help gradient flow)
- [ ] RNNs/LSTMs/GRUs — gating derivations, why they help with gradients, limitations vs attention
- [ ] Temporal Convolutional Networks (TCNs) — dilated causal convolutions, receptive field growth, why they compete with RNNs for sequence tasks
- [ ] Attention & Transformers — derive self-attention (Q/K/V), multi-head attention, positional encoding, why transformers scale better than RNNs
- [ ] Normalization: batchnorm, layernorm, groupnorm — why they work, train/inference differences
- [ ] Optimization in DL: SGD/momentum/RMSprop/Adam — derive update rules; learning rate schedules, warmup, weight decay vs L2
- [ ] Regularization in DL: dropout (derive expectation argument), data augmentation, label smoothing, early stopping
- [ ] Generative models: autoencoders, VAEs (derive ELBO), GANs (minimax objective, mode collapse), diffusion models (forward/reverse process intuition)
- [ ] Self-supervised & contrastive learning: SimCLR-style objectives, why pretext tasks work
- [ ] Transfer learning & fine-tuning strategies: feature extraction vs full fine-tuning, catastrophic forgetting
- [ ] Graph neural networks (light — message passing intuition)
- [ ] Practical training: mixed precision, gradient clipping, debugging a model that won't train
- [ ] Distributed training basics: data parallelism vs model parallelism (light)

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

## 12b. Credit Risk & Credit Scoring
- [ ] Scorecard development: WOE (weight of evidence) transformation
- [ ] Information Value (IV) — feature selection, interpretation thresholds
- [ ] Gini coefficient / AUC-ROC — relationship, when Gini is preferred in credit context
- [ ] Population Stability Index (PSI) — model monitoring, drift detection
- [ ] Partial dependence plots (PDPs) — model interpretability for regulators
- [ ] Logistic regression scorecards vs ML models — regulatory/explainability trade-offs
- [ ] Reject inference
- [ ] Basel/IFRS9 context: PD, LGD, EAD — probability of default modeling

## 12c. Survival Analysis
- [ ] Hazard function, survival function, Kaplan-Meier estimator
- [ ] Cox proportional hazards model — derive partial likelihood
- [ ] Censoring: right/left/interval censoring
- [ ] Time-varying covariates
- [ ] Application to credit: time-to-default modeling
- [ ] Competing risks

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

## 16b. Computer Science Fundamentals
- [ ] Complexity theory: Big-O/Theta/Omega, P vs NP (light)
- [ ] Operating systems basics: processes vs threads, concurrency, memory management
- [ ] Distributed systems intuition: CAP theorem, consistency models

## 16c. Design Patterns
- [ ] SOLID principles
- [ ] Common patterns: Singleton, Factory, Strategy, Observer, Decorator
- [ ] Dependency injection
- [ ] When patterns help vs over-engineering — practical judgment

## 16d. Databases & Data Systems
- [ ] SQL fundamentals: joins, subqueries, window functions
- [ ] Clustered vs unclustered (non-clustered) indexes — storage, trade-offs
- [ ] Query optimization, execution plans (light)
- [ ] Normalization (1NF-3NF), denormalization trade-offs
- [ ] ACID properties, transaction isolation levels
- [ ] SQL vs NoSQL — when each fits, CAP theorem link back to §16b
- [ ] Data warehousing basics: OLTP vs OLAP

## 17. Experimentation & A/B Testing
- [ ] Designing experiments, power analysis
- [ ] Common pitfalls: peeking, novelty effects, network effects
- [ ] Sequential testing, multi-armed bandits

## 18. ML Systems / MLOps (light touch — flag relevance per interview)
- [ ] Training/serving pipelines, feature stores
- [ ] Model monitoring, drift detection
- [ ] Scalability considerations (batch vs online inference)

---

## 19. Philosophy (light — well-roundedness, not core technical prep)
- [ ] Philosophy of mind: the hard problem of consciousness, functionalism vs physicalism
- [ ] Philosophy of causation: Hume on causation, causal realism, links to §12 Causal Inference
- [ ] Philosophy of science: falsifiability (Popper), paradigm shifts (Kuhn), problem of induction
- [ ] Determinism, free will, and their (loose) relevance to model interpretability debates

---

## Gaps Log
*(Running list of things to revisit — add after each session)*
-

## Session Notes
*(Optional: date + topic + key takeaway)*
-
