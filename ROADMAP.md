# Roadmap: ML beginner to pro

The full plan, mirrored from the shared learning-path document. One project per week, Monday to Sunday.

## How this path works

You learn ML by building one new project every week: 41 weekly projects that together cover every major model family, then a 6-week capstone. Each week lists exactly what to learn to finish it: concepts, math, Python libraries, tools, free resources and a clear "done when" target. Learn each item only when the week needs it, then use it straight away.

The plan assumes you are a beginner with little Python and high-school math, studying about 8 to 10 hours a week. At that pace the whole path takes 47 weeks, from 30 November 2026 to late October 2027, with one GitHub push every week.

**The loop for every project**

1. Read the project brief and the "What to learn" table.
2. Study only the listed resources, in short bursts (1 to 2 hours), then go back to the code.
3. Hit each milestone in order and tick it off.
4. Push the code to GitHub with a README that explains the problem, your approach, results and what you would do next.
5. Write a short reflection: what broke, what you learned, what still feels shaky.

**How to adjust**

| If you... | Then |
| --- | --- |
| Already write Python comfortably | Do weeks 1 and 2 together in one week and start week 4 a week early |
| Studied calculus and linear algebra | Skim the math resources; still do the from-scratch parts |
| Have 4 to 5 hours a week | Give each project two weeks and shift the dates; keep the order |
| Have 15+ hours a week | Add the stretch idea from each week's resources, or enter the Kaggle competition linked that week |
| Mainly want LLM and AI apps | Do weeks 1 to 6, 11, 23 to 26 and 32 to 36, then the MLOps weeks |
| Want a research path | Add the [Mathematics for Machine Learning](https://mml-book.github.io/) book and the [d2l.ai](https://d2l.ai/) chapters alongside weeks 23 to 38 |

**Setup (do this once, about 2 hours)**

- [ ] Install Python 3.12 with [uv](https://docs.astral.sh/uv/) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html), plus [VS Code](https://code.visualstudio.com/)
- [ ] Create a [Google Colab](https://colab.research.google.com/) account for free GPUs (needed from Project 6)
- [ ] Create [GitHub](https://github.com/) and [Kaggle](https://www.kaggle.com/) accounts
- [ ] Create the GitHub repo `ml-beginner-to-pro` (layout in Weekly GitHub submission below)

## Model coverage

Every major ML model family gets its own weekly project, in order from simplest to most advanced. Weeks 1 to 3 build the Python and math base; weeks 42 to 47 are the capstone.

| Area | Models and methods | Week |
| --- | --- | --- |
| Regression | Linear regression (from scratch and scikit-learn) | 4 |
| Regression | Polynomial regression, Ridge, Lasso, ElasticNet | 5 |
| Classification | Logistic regression | 6 |
| Classification | k-nearest neighbours (KNN) | 7 |
| Classification | Naive Bayes | 8 |
| Trees | Decision trees | 9 |
| Ensembles | Random forest and bagging | 10 |
| Ensembles | Gradient boosting: XGBoost, LightGBM, CatBoost | 11 |
| Classification | Support vector machines and kernels | 12 |
| Responsible ML | Explainability (SHAP, LIME) and fairness | 13 |
| Ensembles | Voting and stacking, full Kaggle pipeline | 14 |
| Clustering | K-means and hierarchical clustering | 15 |
| Clustering | DBSCAN and Gaussian mixture models | 16 |
| Dimensionality reduction | PCA, t-SNE, UMAP | 17 |
| Anomaly detection | Isolation Forest, Local Outlier Factor, One-Class SVM | 18 |
| Recommenders | Content-based, collaborative filtering, matrix factorization | 19 |
| Pattern mining | Association rules: Apriori, FP-Growth | 20 |
| Time series | ARIMA, SARIMA, exponential smoothing, Prophet | 21 |
| Time series | Gradient boosting with lag features, multi-series forecasting | 22 |
| Neural networks | Perceptron and multilayer perceptron from scratch | 23 |
| Neural networks | MLPs in PyTorch, optimizers, regularization | 24 |
| Computer vision | Convolutional neural networks (CNNs) | 25 |
| Computer vision | Transfer learning with pretrained CNNs | 26 |
| Computer vision | Object detection (YOLO) | 27 |
| Sequence models | RNN, LSTM, GRU | 28 |
| Generative models | Autoencoders and variational autoencoders (VAE) | 29 |
| Generative models | Generative adversarial networks (GANs) | 30 |
| Generative models | Diffusion models | 31 |
| NLP | TF-IDF, word2vec, topic models (LDA) | 32 |
| NLP | Transformer and GPT from scratch | 33 |
| NLP | BERT fine-tuning | 34 |
| LLM apps | Retrieval-augmented generation (RAG) | 35 |
| LLM apps | LoRA fine-tuning and tool-using agents | 36 |
| Reinforcement learning | Multi-armed bandits, Q-learning | 37 |
| Reinforcement learning | Deep Q-Networks, PPO | 38 |
| MLOps | Experiment tracking and model APIs | 39 |
| MLOps | Docker, CI/CD, cloud deployment | 40 |
| MLOps | Monitoring, drift, retraining pipelines | 41 |

Not covered as a full week: graph neural networks and Bayesian models. Add them as stretch projects after the capstone if you want to go further.

## Weekly GitHub submission

Every week ends with a push by Sunday night to one repo, `github.com/aolabodedr/ml-beginner-to-pro`, so progress can be reviewed in one place each Monday. One repo with a folder per week is easier to review than 47 small repos. Apps you deploy (weeks 19, 26, 35, 39 to 41 and the capstone) may live in their own repo, linked from that week's folder.

**Repo layout**

```
ml-beginner-to-pro/
  README.md            <- progress table: week, title, status, link
  week-01-python-basics/
    README.md
    notebook.ipynb or src/
    requirements.txt
    data/README.md     <- where the data comes from (no large files)
    results/           <- charts, metrics.json
  week-02-data-questions/
  ...
```

**Every week folder must contain**

- [ ] `README.md` with: goal of the week, what you built, how to run it, results (numbers and at least one chart), what broke, and one question you still have
- [ ] Code that runs from top to bottom (notebook restarted and re-run before pushing, or a script)
- [ ] `requirements.txt` listing the libraries used
- [ ] Results saved in `results/` (charts as PNG, metrics in a small JSON or table)
- [ ] A link to the data source; no files over 50 MB in git
- [ ] At least 3 commits during the week with clear messages, not one dump on Sunday
- [ ] The root README progress table updated

**How a week is reviewed:** does the code run, does the result meet the week's target, is the README clear, and are the concepts used correctly. Feedback goes back as short notes on what to fix and what to learn next.

## Week-by-week timeline

A new project starts every Monday from 30 November 2026 and is pushed to GitHub by Sunday night; the last week ends 24 October 2027. If you miss a week, shift every later date by one week rather than doubling up. Weeks 4 and 5 fall over the holidays, so a slip there is expected.

| Week | Starts | Stage | Project | Folder |
| --- | --- | --- | --- | --- |
| 1 | 30 Nov 2026 | Foundations | Command-line budget tracker | `week-01-budget-tracker` |
| 2 | 7 Dec 2026 | Foundations | Explore a real dataset | `week-02-data-exploration` |
| 3 | 14 Dec 2026 | Foundations | Gradient descent from scratch | `week-03-gradient-descent` |
| 4 | 21 Dec 2026 | Supervised | House prices: linear regression | `week-04-linear-regression` |
| 5 | 28 Dec 2026 | Supervised | Fuel efficiency: polynomial, Ridge, Lasso | `week-05-regularization` |
| 6 | 4 Jan 2027 | Supervised | Heart disease: logistic regression | `week-06-logistic-regression` |
| 7 | 11 Jan 2027 | Supervised | Digit recognizer: KNN | `week-07-knn` |
| 8 | 18 Jan 2027 | Supervised | Spam filter: Naive Bayes | `week-08-naive-bayes` |
| 9 | 25 Jan 2027 | Supervised | Bank marketing: decision trees | `week-09-decision-trees` |
| 10 | 1 Feb 2027 | Supervised | Credit default: random forest | `week-10-random-forest` |
| 11 | 8 Feb 2027 | Supervised | Churn: XGBoost, LightGBM, CatBoost | `week-11-gradient-boosting` |
| 12 | 15 Feb 2027 | Supervised | Tumour classifier: SVM | `week-12-svm` |
| 13 | 22 Feb 2027 | Supervised | Income: explainability and fairness | `week-13-explainability` |
| 14 | 1 Mar 2027 | Supervised | Kaggle House Prices: stacking | `week-14-stacking` |
| 15 | 8 Mar 2027 | Unsupervised | Customer segments: k-means, hierarchical | `week-15-kmeans` |
| 16 | 15 Mar 2027 | Unsupervised | Earthquakes: DBSCAN, GMM | `week-16-dbscan-gmm` |
| 17 | 22 Mar 2027 | Unsupervised | Images: PCA, t-SNE, UMAP | `week-17-dim-reduction` |
| 18 | 29 Mar 2027 | Unsupervised | Fraud: anomaly detection | `week-18-anomaly-detection` |
| 19 | 5 Apr 2027 | Unsupervised | Movie recommender | `week-19-recommender` |
| 20 | 12 Apr 2027 | Unsupervised | Market basket: association rules | `week-20-association-rules` |
| 21 | 19 Apr 2027 | Time series | Demand: ARIMA, SARIMA, Prophet | `week-21-classical-forecasting` |
| 22 | 26 Apr 2027 | Time series | Store sales: LightGBM forecasting | `week-22-ml-forecasting` |
| 23 | 3 May 2027 | Deep learning | Neural network from scratch | `week-23-nn-from-scratch` |
| 24 | 10 May 2027 | Deep learning | Fashion-MNIST in PyTorch | `week-24-pytorch-mlp` |
| 25 | 17 May 2027 | Deep learning | CIFAR-10 CNN | `week-25-cnn` |
| 26 | 24 May 2027 | Deep learning | Transfer learning app | `week-26-transfer-learning` |
| 27 | 31 May 2027 | Deep learning | Object detection: YOLO | `week-27-object-detection` |
| 28 | 7 Jun 2027 | Deep learning | Sentiment and text: LSTM | `week-28-lstm` |
| 29 | 14 Jun 2027 | Deep learning | Autoencoders and VAE | `week-29-autoencoders` |
| 30 | 21 Jun 2027 | Deep learning | GAN | `week-30-gan` |
| 31 | 28 Jun 2027 | Deep learning | Diffusion model | `week-31-diffusion` |
| 32 | 5 Jul 2027 | NLP and LLMs | Topics and embeddings | `week-32-classic-nlp` |
| 33 | 12 Jul 2027 | NLP and LLMs | Mini-GPT from scratch | `week-33-mini-gpt` |
| 34 | 19 Jul 2027 | NLP and LLMs | Fine-tuned BERT | `week-34-bert` |
| 35 | 26 Jul 2027 | NLP and LLMs | RAG document assistant | `week-35-rag` |
| 36 | 2 Aug 2027 | NLP and LLMs | LoRA fine-tune and agent | `week-36-lora-agent` |
| 37 | 9 Aug 2027 | Reinforcement learning | Bandits and Q-learning | `week-37-q-learning` |
| 38 | 16 Aug 2027 | Reinforcement learning | DQN and PPO | `week-38-deep-rl` |
| 39 | 23 Aug 2027 | MLOps | MLflow and FastAPI | `week-39-tracking-api` |
| 40 | 30 Aug 2027 | MLOps | Docker, CI/CD, deploy | `week-40-docker-ci` |
| 41 | 6 Sep 2027 | MLOps | Monitoring and retraining | `week-41-monitoring` |
| 42 | 13 Sep 2027 | Capstone | Proposal and data collection | `week-42-capstone-proposal` |
| 43 | 20 Sep 2027 | Capstone | Cleaning, EDA and baseline | `week-43-capstone-baseline` |
| 44 | 27 Sep 2027 | Capstone | Stronger models and experiments | `week-44-capstone-models` |
| 45 | 4 Oct 2027 | Capstone | Error analysis and app | `week-45-capstone-app` |
| 46 | 11 Oct 2027 | Capstone | Deploy with tests, CI and monitoring | `week-46-capstone-deploy` |
| 47 | 18 Oct 2027 | Capstone | Write-up, model card, demo video | `week-47-capstone-showcase` |

## Stage 1: Foundations (weeks 1 to 3)

Three weeks to get Python, data handling and the core math in place, so every later week can focus on the model.

### Week 1 (30 Nov to 6 Dec 2026): Command-line budget tracker

- **Build:** a Python program that records expenses, saves them to a CSV file and prints a monthly summary by category.
- **Learn:** variables, data types, lists, dicts, loops, conditionals, functions, reading and writing files, handling errors.
- **Math:** percentages and averages.
- **Use:** Python 3.12, VS Code, terminal, git and GitHub.
- **Resources:** [Python for Everybody](https://www.py4e.com/) chapters 1 to 10, Kaggle Learn [Python](https://www.kaggle.com/learn/python).
- **Done when:** the tracker runs from the terminal, survives bad input, and the summary is correct.

### Week 2 (7 to 13 Dec 2026): Explore a real dataset

- **Build:** a notebook that answers 5 questions about a dataset you like (football, music, World Bank, or your own data) with numbers and charts.
- **Learn:** NumPy arrays, pandas (load, filter, groupby, merge, missing values), matplotlib and seaborn.
- **Math:** mean, median, standard deviation, percentiles, distributions, correlation.
- **Use:** Jupyter or Google Colab.
- **Resources:** Kaggle Learn [Pandas](https://www.kaggle.com/learn/pandas) and [Data Visualization](https://www.kaggle.com/learn/data-visualization), [Khan Academy statistics](https://www.khanacademy.org/math/statistics-probability).
- **Done when:** someone else can read the notebook and understand each answer without you.

### Week 3 (14 to 20 Dec 2026): Gradient descent from scratch

- **Build:** a NumPy program that finds the minimum of a function and fits a straight line to points using gradient descent, with a plot of the loss falling.
- **Learn:** what a model, a loss and optimization are; learning rate; convergence.
- **Math:** vectors, dot product, matrices, derivatives, partial derivatives, the gradient, basic probability.
- **Use:** NumPy, matplotlib.
- **Resources:** 3Blue1Brown [Essence of Linear Algebra](https://www.3blue1brown.com/topics/linear-algebra) episodes 1 to 4 and [Essence of Calculus](https://www.3blue1brown.com/topics/calculus) episodes 1 to 4, [Khan Academy probability](https://www.khanacademy.org/math/statistics-probability/probability-library).
- **Done when:** your line matches `numpy.polyfit` closely and you can explain each update step on paper.

## Stage 2: Supervised learning (weeks 4 to 14)

One model family per week on a real dataset. Each week, start with a simple baseline, then the new model, and compare them in a results table.

### Week 4 (21 to 27 Dec 2026): House price predictor with linear regression

- **Build:** predict prices on California Housing (`sklearn.datasets.fetch_california_housing`), first with your own NumPy linear regression, then scikit-learn.
- **Learn:** supervised learning, features and target, train/test split, baseline model, MSE, RMSE, R squared, feature scaling.
- **Math:** matrix form of linear regression, the normal equation, gradient of MSE.
- **Use:** NumPy, scikit-learn `LinearRegression`, `StandardScaler`.
- **Resources:** [Google ML Crash Course](https://developers.google.com/machine-learning/crash-course) linear regression module, [StatQuest](https://www.youtube.com/@statquest) linear regression videos, Ng's [Machine Learning Specialization](https://www.coursera.org/specializations/machine-learning-introduction) course 1 weeks 1 to 2 (audit free).
- **Done when:** your model is within 1% of scikit-learn's RMSE and both beat the average-price baseline.

### Week 5 (28 Dec 2026 to 3 Jan 2027): Fuel efficiency with polynomial regression and regularization

- **Build:** predict car fuel efficiency on [Auto MPG](https://archive.ics.uci.edu/dataset/9/auto+mpg) and find the best model complexity.
- **Learn:** overfitting and underfitting, bias-variance trade-off, polynomial features, Ridge (L2), Lasso (L1), ElasticNet, k-fold cross-validation, learning curves.
- **Math:** norms of a vector, how a penalty term changes the loss.
- **Use:** scikit-learn `PolynomialFeatures`, `Ridge`, `Lasso`, `ElasticNet`, `cross_val_score`, `GridSearchCV`.
- **Resources:** StatQuest Ridge, Lasso and ElasticNet videos, [scikit-learn linear models guide](https://scikit-learn.org/stable/modules/linear_model.html).
- **Done when:** a plot shows validation error against polynomial degree and alpha, and you justify your pick.

### Week 6 (4 to 10 Jan 2027): Heart disease classifier with logistic regression

- **Build:** predict heart disease on the [UCI Heart Disease dataset](https://archive.ics.uci.edu/dataset/45/heart+disease).
- **Learn:** classification, decision boundary, predicted probabilities, thresholds, confusion matrix, accuracy, precision, recall, F1, ROC AUC.
- **Math:** sigmoid function, log-loss (cross-entropy), odds and log-odds.
- **Use:** scikit-learn `LogisticRegression`, `classification_report`, `RocCurveDisplay`.
- **Resources:** Ng's Machine Learning Specialization course 1 week 3, StatQuest logistic regression and ROC/AUC videos.
- **Done when:** you report cross-validated AUC and explain which threshold a doctor would prefer and why.

### Week 7 (11 to 17 Jan 2027): Handwritten digit recognizer with KNN

- **Build:** classify digits from `sklearn.datasets.load_digits`, with your own KNN first, then scikit-learn.
- **Learn:** instance-based learning, choosing k, distance metrics, why scaling matters, the curse of dimensionality, multi-class metrics.
- **Math:** Euclidean and Manhattan distance, majority voting.
- **Use:** scikit-learn `KNeighborsClassifier`, `Pipeline`.
- **Resources:** StatQuest k-nearest neighbors, [scikit-learn neighbors guide](https://scikit-learn.org/stable/modules/neighbors.html).
- **Done when:** k is tuned with cross-validation, you show 10 misclassified digits, and your KNN matches scikit-learn.

### Week 8 (18 to 24 Jan 2027): SMS spam filter with Naive Bayes

- **Build:** a spam filter on the [SMS Spam Collection](https://archive.ics.uci.edu/dataset/228/sms+spam+collection).
- **Learn:** text as features, bag of words, TF-IDF, the naive independence assumption, Laplace smoothing, class imbalance.
- **Math:** Bayes' theorem, conditional probability, log probabilities.
- **Use:** scikit-learn `CountVectorizer`, `TfidfVectorizer`, `MultinomialNB`.
- **Resources:** StatQuest Naive Bayes, 3Blue1Brown [Bayes theorem](https://www.3blue1brown.com/lessons/bayes-theorem).
- **Done when:** your from-scratch Naive Bayes matches scikit-learn and spam F1 is above 0.9.

### Week 9 (25 to 31 Jan 2027): Bank marketing predictor with decision trees

- **Build:** predict who subscribes to a term deposit on [Bank Marketing](https://archive.ics.uci.edu/dataset/222/bank+marketing).
- **Learn:** how trees split, depth and leaf size, pruning, overfitting in trees, handling categorical features.
- **Math:** entropy, information gain, Gini impurity.
- **Use:** scikit-learn `DecisionTreeClassifier`, `plot_tree`, `OneHotEncoder`.
- **Resources:** StatQuest decision trees, Ng's Machine Learning Specialization course 2 week 4.
- **Done when:** you show the tree, explain its top 3 splits in plain English, and compare 3 depths.

### Week 10 (1 to 7 Feb 2027): Credit default predictor with random forests

- **Build:** predict credit card default on [Default of Credit Card Clients](https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients).
- **Learn:** bootstrap sampling, bagging, random feature subsets, out-of-bag error, feature and permutation importance.
- **Math:** variance reduction by averaging.
- **Use:** scikit-learn `RandomForestClassifier`, `BaggingClassifier`, `permutation_importance`.
- **Resources:** StatQuest random forests, [scikit-learn ensembles guide](https://scikit-learn.org/stable/modules/ensemble.html).
- **Done when:** the forest beats a single tree and you report out-of-bag score and top features.

### Week 11 (8 to 14 Feb 2027): Customer churn with gradient boosting

- **Build:** predict churn on [Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) and compare three boosting libraries.
- **Learn:** boosting, fitting residuals, learning rate and number of trees, early stopping, hyperparameter search.
- **Math:** gradient boosting as gradient descent on the loss.
- **Use:** XGBoost, LightGBM, CatBoost, Optuna.
- **Resources:** StatQuest gradient boosting and XGBoost series, [XGBoost docs](https://xgboost.readthedocs.io/), Kaggle Learn [Intermediate ML](https://www.kaggle.com/learn/intermediate-machine-learning).
- **Done when:** one table compares the 3 libraries on AUC and training time after tuning.

### Week 12 (15 to 21 Feb 2027): Tumour classifier with support vector machines

- **Build:** classify tumours on `sklearn.datasets.load_breast_cancer`, plus 2D toy datasets (moons, circles) to see kernels at work.
- **Learn:** margins, support vectors, soft margin and C, kernels (linear, polynomial, RBF), gamma.
- **Math:** distance from a point to a hyperplane, hinge loss, the kernel trick.
- **Use:** scikit-learn `SVC`, `make_moons`, `make_circles`.
- **Resources:** StatQuest support vector machines, [scikit-learn SVM guide](https://scikit-learn.org/stable/modules/svm.html).
- **Done when:** decision boundary plots for 3 kernels and a tuned SVM compared with week 6's logistic regression.

### Week 13 (22 to 28 Feb 2027): Income prediction with explainability and fairness

- **Build:** predict income on [UCI Adult](https://archive.ics.uci.edu/dataset/2/adult), explain the model and audit it for bias across sex and race.
- **Learn:** global vs local explanations, SHAP, LIME, partial dependence, fairness metrics (demographic parity, equal opportunity), mitigation.
- **Math:** Shapley values (intuition), conditional rates per group.
- **Use:** SHAP, LIME, Fairlearn.
- **Resources:** [Interpretable Machine Learning](https://christophm.github.io/interpretable-ml-book/) chapters on SHAP and LIME, [Fairlearn user guide](https://fairlearn.org/).
- **Done when:** a one-page report shows what drives predictions and where the model treats groups differently.

### Week 14 (1 to 7 Mar 2027): Kaggle House Prices with stacking

- **Build:** a full submission to Kaggle [House Prices](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques) using everything from weeks 4 to 13.
- **Learn:** feature engineering, `Pipeline` and `ColumnTransformer`, avoiding data leakage, voting and stacking ensembles.
- **Math:** log transform of skewed targets, why averaging diverse models helps.
- **Use:** scikit-learn `StackingRegressor`, `VotingRegressor`, Kaggle notebooks.
- **Resources:** Kaggle Learn [Feature Engineering](https://www.kaggle.com/learn/feature-engineering), top public notebooks on the competition.
- **Done when:** a stacked model beats your best single model on cross-validation and you have a leaderboard score.

## Stage 3: Unsupervised learning, recommenders and time series (weeks 15 to 22)

These weeks cover problems with no labels, or where order in time matters.

### Week 15 (8 to 14 Mar 2027): Customer segmentation with k-means and hierarchical clustering

- **Build:** segment shoppers on the [Mall Customers dataset](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python) and write a marketing persona for each segment.
- **Learn:** unsupervised learning, k-means, choosing k (elbow, silhouette), agglomerative clustering, linkage types, dendrograms.
- **Math:** centroids, within-cluster sum of squares, distance matrices.
- **Use:** scikit-learn `KMeans`, `AgglomerativeClustering`, SciPy `dendrogram`.
- **Resources:** StatQuest k-means and hierarchical clustering, [scikit-learn clustering guide](https://scikit-learn.org/stable/modules/clustering.html).
- **Done when:** both methods are compared and each segment has a clear, named persona.

### Week 16 (15 to 21 Mar 2027): Earthquake hotspots with DBSCAN and Gaussian mixtures

- **Build:** cluster a year of earthquake locations from the [USGS earthquake catalog](https://earthquake.usgs.gov/earthquakes/search/) and plot clusters on a map.
- **Learn:** density-based clustering, eps and min\_samples, noise points, soft clustering with Gaussian mixtures, choosing components with BIC.
- **Math:** the normal distribution in several dimensions, covariance, the expectation-maximization (EM) algorithm (intuition).
- **Use:** scikit-learn `DBSCAN`, `GaussianMixture`, folium or plotly maps.
- **Resources:** StatQuest DBSCAN and Gaussian mixture videos.
- **Done when:** a map compares k-means, DBSCAN and GMM, and you say which fits this data best.

### Week 17 (22 to 28 Mar 2027): Visualizing and compressing images with PCA, t-SNE and UMAP

- **Build:** compress Fashion-MNIST images with PCA and draw 2D maps of the dataset with PCA, t-SNE and UMAP.
- **Learn:** dimensionality reduction, explained variance, reconstruction error, linear vs non-linear embeddings.
- **Math:** eigenvectors and eigenvalues, covariance matrix, singular value decomposition.
- **Use:** scikit-learn `PCA`, `TSNE`, umap-learn.
- **Resources:** 3Blue1Brown Essence of Linear Algebra episodes 9 to 14, StatQuest PCA and t-SNE videos.
- **Done when:** you show images rebuilt from 10, 50 and 150 components and compare the 3 maps.

### Week 18 (29 Mar to 4 Apr 2027): Credit card fraud with anomaly detection

- **Build:** detect fraud on the [Credit Card Fraud dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud), unsupervised first, then supervised.
- **Learn:** outliers vs novelties, Isolation Forest, Local Outlier Factor, One-Class SVM, extreme class imbalance, resampling (SMOTE), PR-AUC.
- **Math:** z-scores, path length in random trees, precision-recall curves.
- **Use:** scikit-learn `IsolationForest`, `LocalOutlierFactor`, `OneClassSVM`; imbalanced-learn.
- **Resources:** [scikit-learn outlier detection guide](https://scikit-learn.org/stable/modules/outlier_detection.html), StatQuest precision-recall videos.
- **Done when:** a table compares PR-AUC for 3 unsupervised and 1 supervised model.

### Week 19 (5 to 11 Apr 2027): Movie recommender

- **Build:** a recommender on [MovieLens](https://grouplens.org/datasets/movielens/) (latest-small) with a small Streamlit page.
- **Learn:** content-based filtering, user-user and item-item collaborative filtering, matrix factorization, cold start, precision@k.
- **Math:** cosine similarity, low-rank matrix factorization.
- **Use:** pandas, SciPy sparse matrices, scikit-surprise, Streamlit.
- **Resources:** Google [Recommendation Systems course](https://developers.google.com/machine-learning/recommendation), Ng's Machine Learning Specialization course 3 week 2.
- **Done when:** matrix factorization beats a popularity baseline on precision@10 and the demo runs.

### Week 20 (12 to 18 Apr 2027): Market basket analysis with association rules

- **Build:** find products bought together in the [Online Retail dataset](https://archive.ics.uci.edu/dataset/352/online+retail).
- **Learn:** frequent itemsets, Apriori, FP-Growth, support, confidence, lift.
- **Math:** joint and conditional probability.
- **Use:** mlxtend.
- **Resources:** [mlxtend frequent patterns guide](https://rasbt.github.io/mlxtend/user_guide/frequent_patterns/apriori/).
- **Done when:** you list the top 10 rules and turn 3 into concrete shop suggestions.

### Week 21 (19 to 25 Apr 2027): Electricity demand forecast with classical time series

- **Build:** forecast monthly airline passengers or hourly electricity demand (for example [PJM energy data](https://www.kaggle.com/datasets/robikscube/hourly-energy-consumption)).
- **Learn:** trend, seasonality, stationarity, differencing, autocorrelation, ARIMA and SARIMA, exponential smoothing, Prophet, walk-forward backtesting.
- **Math:** moving averages, autocorrelation function, MAPE.
- **Use:** statsmodels, Prophet.
- **Resources:** [Forecasting: Principles and Practice](https://otexts.com/fpp3/) chapters 1 to 9 (free online).
- **Done when:** SARIMA and Prophet both beat a seasonal naive forecast in a backtest.

### Week 22 (26 Apr to 2 May 2027): Store sales forecast with machine learning

- **Build:** forecast many product series in Kaggle's [Store Sales](https://www.kaggle.com/competitions/store-sales-time-series-forecasting) competition.
- **Learn:** lag and rolling features, calendar and holiday features, time-based cross-validation, global models across many series.
- **Math:** RMSLE, why random splits leak future information.
- **Use:** LightGBM, pandas time features, scikit-learn `TimeSeriesSplit`.
- **Resources:** Kaggle Learn [Time Series](https://www.kaggle.com/learn/time-series).
- **Done when:** LightGBM beats your week 21 approach on the same backtest and you submit to Kaggle.

## Stage 4: Deep learning (weeks 23 to 31)

From a neural network you write by hand to models that see, read sequences and generate images. From week 25, use a free Colab GPU.

### Week 23 (3 to 9 May 2027): Neural network from scratch

- **Build:** a 2-layer neural network in pure NumPy that classifies MNIST digits.
- **Learn:** perceptron, multilayer perceptron, activations (sigmoid, ReLU, softmax), forward and backward pass, mini-batches, epochs.
- **Math:** chain rule, matrix calculus for one layer, cross-entropy loss, numerical gradient checking.
- **Use:** NumPy only.
- **Resources:** 3Blue1Brown [Neural Networks series](https://www.3blue1brown.com/topics/neural-networks), Karpathy [Neural Networks: Zero to Hero](https://karpathy.ai/zero-to-hero.html) lecture 1 (micrograd).
- **Done when:** 95%+ test accuracy and your backprop passes a numerical gradient check.

### Week 24 (10 to 16 May 2027): Fashion item classifier in PyTorch

- **Build:** rebuild your network in PyTorch and train it on Fashion-MNIST.
- **Learn:** tensors, autograd, `nn.Module`, `DataLoader`, training and validation loops, SGD vs Adam, dropout, batch norm, weight decay, learning rate schedules.
- **Math:** momentum and adaptive learning rates.
- **Use:** PyTorch, torchvision, TensorBoard or Weights and Biases.
- **Resources:** [PyTorch Learn the Basics](https://pytorch.org/tutorials/beginner/basics/intro.html), [Dive into Deep Learning](https://d2l.ai/) chapters 3 to 5.
- **Done when:** 88%+ test accuracy and logged curves for 3 settings.

### Week 25 (17 to 23 May 2027): CIFAR-10 image classifier with a CNN

- **Build:** a convolutional network trained from scratch on CIFAR-10.
- **Learn:** convolutions, filters, padding, stride, pooling, feature maps, data augmentation, residual connections.
- **Math:** convolution as a sliding dot product, counting parameters per layer.
- **Use:** PyTorch, torchvision transforms, Colab GPU.
- **Resources:** [CS231n notes](https://cs231n.github.io/) on CNNs, Dive into Deep Learning chapters 7 and 8.
- **Done when:** 80%+ test accuracy and a plot of learned first-layer filters.

### Week 26 (24 to 30 May 2027): Your own image classifier app with transfer learning

- **Build:** collect 3 to 5 classes of your own photos (for example local foods or plant leaves), fine-tune a pretrained model and publish it on [Hugging Face Spaces](https://huggingface.co/spaces).
- **Learn:** transfer learning, freezing and unfreezing layers, fine-tuning, error analysis.
- **Math:** why pretrained features transfer.
- **Use:** timm or fastai, Gradio, Hugging Face Hub.
- **Resources:** fast.ai [Practical Deep Learning](https://course.fast.ai/) lessons 1 and 2, [Gradio quickstart](https://www.gradio.app/guides/quickstart).
- **Done when:** a public app link works and you show the 10 worst mistakes.

### Week 27 (31 May to 6 Jun 2027): Object detector with YOLO

- **Build:** train a detector on a dataset from [Roboflow Universe](https://universe.roboflow.com/) or your own labelled photos, and run it on a video.
- **Learn:** bounding boxes, anchors, non-maximum suppression, detection vs segmentation, labelling data.
- **Math:** intersection over union (IoU), mean average precision (mAP).
- **Use:** Ultralytics YOLO, Roboflow or Label Studio.
- **Resources:** [Ultralytics docs](https://docs.ultralytics.com/), CS231n detection lecture notes.
- **Done when:** you report mAP@0.5 and share a short demo video.

### Week 28 (7 to 13 Jun 2027): Movie review sentiment and text generator with LSTMs

- **Build:** an LSTM sentiment classifier on [IMDB reviews](https://huggingface.co/datasets/stanfordnlp/imdb), plus a character-level text generator.
- **Learn:** sequence data, embedding layers, RNNs, LSTMs and GRUs, padding and packing, vanishing gradients, sampling with temperature.
- **Math:** recurrence, LSTM gates, backpropagation through time.
- **Use:** PyTorch `nn.LSTM`, `nn.GRU`.
- **Resources:** Chris Olah [Understanding LSTMs](https://colah.github.io/posts/2015-08-Understanding-LSTMs/), Dive into Deep Learning chapters 9 and 10.
- **Done when:** the LSTM beats a TF-IDF baseline and you share generated text samples.

### Week 29 (14 to 20 Jun 2027): Image denoiser and digit generator with autoencoders

- **Build:** a denoising autoencoder and a variational autoencoder (VAE) on MNIST.
- **Learn:** encoder and decoder, latent space, reconstruction loss, VAEs, sampling new data.
- **Math:** KL divergence, the reparameterization trick.
- **Use:** PyTorch.
- **Resources:** Dive into Deep Learning generative chapters, [PyTorch examples VAE](https://github.com/pytorch/examples/tree/main/vae).
- **Done when:** you show noisy, cleaned and original images, plus a grid that walks across the latent space.

### Week 30 (21 to 27 Jun 2027): Fashion item generator with a GAN

- **Build:** a DCGAN that generates Fashion-MNIST items.
- **Learn:** generator and discriminator, adversarial training, mode collapse, training tricks.
- **Math:** the minimax objective, binary cross-entropy for both players.
- **Use:** PyTorch.
- **Resources:** [PyTorch DCGAN tutorial](https://pytorch.org/tutorials/beginner/dcgan_faces_tutorial.html).
- **Done when:** a GIF shows samples improving across epochs.

### Week 31 (28 Jun to 4 Jul 2027): Tiny diffusion model

- **Build:** train a small diffusion model (DDPM) on MNIST or Fashion-MNIST, then generate images with a pretrained Stable Diffusion pipeline.
- **Learn:** forward noising, reverse denoising, noise schedules, U-Net, guidance.
- **Math:** Gaussian noise, predicting noise with a mean squared error loss.
- **Use:** PyTorch, Hugging Face diffusers.
- **Resources:** Hugging Face [Diffusion Models Course](https://huggingface.co/learn/diffusion-course).
- **Done when:** your own model produces recognisable digits and you compare it with your GAN and VAE.

## Stage 5: NLP, transformers and LLMs (weeks 32 to 36)

From classic text features to building and fine-tuning the models behind today's AI assistants.

### Week 32 (5 to 11 Jul 2027): News topic explorer with classic NLP

- **Build:** find topics in a news corpus (for example [20 Newsgroups](https://scikit-learn.org/stable/datasets/real_world.html#newsgroups-dataset) or BBC News) and explore word embeddings.
- **Learn:** tokenization, stop words, stemming and lemmatization, TF-IDF, word2vec and GloVe embeddings, LDA topic modelling, named entity recognition.
- **Math:** vector arithmetic on embeddings, Dirichlet distribution (intuition).
- **Use:** spaCy, gensim, pyLDAvis.
- **Resources:** [spaCy course](https://course.spacy.io/), Jay Alammar [The Illustrated Word2vec](https://jalammar.github.io/illustrated-word2vec/).
- **Done when:** each topic has a sensible label and you show 5 working word analogies.

### Week 33 (12 to 18 Jul 2027): Mini-GPT from scratch

- **Build:** a small character-level GPT trained on Shakespeare (or texts in a language you speak).
- **Learn:** self-attention, multi-head attention, positional encoding, causal masking, layer norm, residual streams, tokenizers.
- **Math:** scaled dot-product attention, softmax over scores.
- **Use:** PyTorch.
- **Resources:** Karpathy [Let's build GPT](https://karpathy.ai/zero-to-hero.html) (Zero to Hero), Jay Alammar [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/), 3Blue1Brown attention videos.
- **Done when:** the model generates plausible text and you can draw the attention block from memory.

### Week 34 (19 to 25 Jul 2027): Fine-tuned BERT classifier

- **Build:** fine-tune DistilBERT on a text classification or named-entity task and push the model to the Hugging Face Hub.
- **Learn:** pretraining vs fine-tuning, encoder models, subword tokenizers, the Trainer API, evaluation.
- **Math:** masked language modelling objective.
- **Use:** Hugging Face `transformers`, `datasets`, `evaluate`.
- **Resources:** [Hugging Face LLM Course](https://huggingface.co/learn) chapters 1 to 4.
- **Done when:** it beats your week 28 LSTM on the same data and the model page is public.

### Week 35 (26 Jul to 1 Aug 2027): Document Q&A assistant with RAG

- **Build:** an assistant that answers questions about documents you choose (handbook, lecture notes, PDFs) and cites its sources.
- **Learn:** sentence embeddings, chunking, vector databases, retrieval, prompting, retrieval-augmented generation, hallucination, LLM evaluation.
- **Math:** cosine similarity in high dimensions, recall@k.
- **Use:** sentence-transformers, Chroma or FAISS, an LLM API or a small local model, Streamlit or Gradio.
- **Resources:** Hugging Face LLM Course RAG chapters, [Chroma docs](https://docs.trychroma.com/).
- **Done when:** it answers at least 24 of your 30 test questions correctly with citations.

### Week 36 (2 to 8 Aug 2027): Fine-tune a small LLM with LoRA and build an agent

- **Build:** fine-tune a small open model (around 1B parameters) with LoRA on an instruction dataset, then give an LLM two tools (a calculator and a search over your week 35 documents).
- **Learn:** instruction tuning, parameter-efficient fine-tuning, quantization, tool calling, agent loops.
- **Math:** low-rank matrices (why LoRA uses so few parameters).
- **Use:** Hugging Face PEFT, TRL, bitsandbytes, Colab GPU.
- **Resources:** [PEFT docs](https://huggingface.co/docs/peft), Hugging Face [Agents Course](https://huggingface.co/learn/agents-course).
- **Done when:** a before and after comparison on 20 prompts shows the fine-tune helped, and the agent uses both tools correctly.

## Stage 6: Reinforcement learning (weeks 37 to 38)

Agents that learn by trial and error from rewards instead of labelled examples.

### Week 37 (9 to 15 Aug 2027): Taxi agent with bandits and Q-learning

- **Build:** solve a multi-armed bandit problem, then train a Q-learning agent on Gymnasium's Taxi and FrozenLake.
- **Learn:** agents, states, actions, rewards, Markov decision processes, exploration vs exploitation, epsilon-greedy, UCB, value and Q-functions.
- **Math:** the Bellman equation, discounted returns, expected value.
- **Use:** [Gymnasium](https://gymnasium.farama.org/), NumPy.
- **Resources:** Hugging Face [Deep RL Course](https://huggingface.co/learn/deep-rl-course) units 1 and 2, Sutton and Barto [Reinforcement Learning: An Introduction](http://incompleteideas.net/book/the-book-2nd.html) chapters 2 and 6 (free).
- **Done when:** the Taxi agent reaches the optimal average reward and you plot learning curves.

### Week 38 (16 to 22 Aug 2027): Lunar lander with deep RL

- **Build:** a DQN for CartPole written yourself, then a PPO agent that lands LunarLander.
- **Learn:** deep Q-networks, experience replay, target networks, policy gradients, actor-critic, PPO.
- **Math:** policy gradient theorem (intuition), advantage estimates.
- **Use:** PyTorch, Gymnasium, Stable-Baselines3.
- **Resources:** Hugging Face Deep RL Course units 3 and 8, [Stable-Baselines3 docs](https://stable-baselines3.readthedocs.io/).
- **Done when:** CartPole averages 475+ and LunarLander averages 200+, with a video of a landing.

## Stage 7: MLOps and deployment (weeks 39 to 41)

Take the week 11 churn model (or any model you like) and run it like a real product.

### Week 39 (23 to 29 Aug 2027): Tracked experiments and a model API

- **Build:** log all churn training runs in MLflow, register the best model and serve it from a FastAPI `/predict` endpoint.
- **Learn:** experiment tracking, model registry, reproducibility, REST APIs, input validation.
- **Math:** none new.
- **Use:** MLflow, FastAPI, pydantic, uvicorn.
- **Resources:** [MLflow docs](https://mlflow.org/docs/latest/), [FastAPI tutorial](https://fastapi.tiangolo.com/tutorial/), [Made With ML](https://madewithml.com/).
- **Done when:** one command trains and logs a run, and the API returns predictions locally.

### Week 40 (30 Aug to 5 Sep 2027): Docker, CI/CD and cloud deployment

- **Build:** tests for data, model and API, a Docker image, a GitHub Actions workflow and a live deployment.
- **Learn:** unit and integration tests, containers, continuous integration and delivery, environment secrets.
- **Math:** none new.
- **Use:** pytest, Docker, GitHub Actions, a free host (Render, Fly.io or Hugging Face Spaces with Docker).
- **Resources:** [Docker getting started](https://docs.docker.com/get-started/), [GitHub Actions docs](https://docs.github.com/actions), DataTalksClub [MLOps Zoomcamp](https://github.com/DataTalksClub/mlops-zoomcamp).
- **Done when:** every push runs the tests automatically and the live URL returns predictions.

### Week 41 (6 to 12 Sep 2027): Monitoring, drift and automated retraining

- **Build:** simulate a month of new data, detect drift, and trigger retraining with a scheduled pipeline.
- **Learn:** data drift vs concept drift, data validation, monitoring dashboards, orchestration.
- **Math:** Kolmogorov-Smirnov test, population stability index.
- **Use:** Evidently, Prefect.
- **Resources:** [Evidently docs](https://docs.evidentlyai.com/), MLOps Zoomcamp monitoring and orchestration modules.
- **Done when:** a drift report flags the shift and the pipeline retrains and re-registers the model.

## Capstone: your own end-to-end ML product (weeks 42 to 47)

The capstone is a real problem you choose, solved end to end, with data you collect yourself and a deployed product someone else can use. It is the project you show employers or clients.

**Pick one idea (or your own)**

- A crop or plant disease detector from phone photos, with an app farmers can try
- A document assistant for a real organization's policies, with measured answer accuracy
- A price or demand forecaster for a local market using data you scrape weekly
- A transaction categorizer and spending forecaster for personal finance data
- A speech or translation tool for a language underserved by existing models

**What it must include**

| Requirement | Evidence in the repo |
| --- | --- |
| A clear problem and user | Proposal with the problem, who it helps and the success metric |
| Your own data | Collection script or process, data README, ethics and privacy note |
| A baseline and at least 2 stronger approaches | Experiment log in MLflow or Weights and Biases with a comparison table |
| Error analysis | Notebook showing where the model fails and why |
| A deployed product | Public app or API link |
| Engineering quality | Tests, CI on every push, Dockerfile, one-command setup |
| Monitoring | Drift or quality report and a plan for retraining |
| Communication | Model card, final README, 3-minute demo video, a blog or LinkedIn post |

**Weekly plan:** week 42 proposal and data collection, week 43 cleaning, EDA and baseline, week 44 stronger models and experiments, week 45 error analysis and app, week 46 deployment with tests, CI and monitoring, week 47 write-up, model card and demo video. Most capstones need one extra skill, such as web scraping (`requests`, BeautifulSoup) or labelling ([Label Studio](https://labelstud.io/)); learn it in week 42.

**Done when** a stranger can open your link, use the product, read the README and understand the problem, your approach, the results and the limits.

## Free resource library

These are the core resources referenced above, grouped by what they teach. Use them as references when a project needs them, not as courses to finish front to back.

| Resource | Teaches | Weeks |
| --- | --- | --- |
| [Python for Everybody](https://www.py4e.com/) | Python from zero | 1 |
| [Kaggle Learn](https://www.kaggle.com/learn) | Python, pandas, visualization, intermediate ML, feature engineering, time series | 1 to 22 |
| [Khan Academy](https://www.khanacademy.org/math) | Statistics, probability, algebra refreshers | 2 to 8 |
| [3Blue1Brown](https://www.3blue1brown.com/) | Linear algebra, calculus, neural networks and attention, visually | 3, 17, 23, 33 |
| [StatQuest](https://www.youtube.com/@statquest) | Short, clear explanations of every classical ML algorithm | 4 to 21 |
| [Google ML Crash Course](https://developers.google.com/machine-learning/crash-course) | Core ML concepts with exercises | 4 to 6 |
| [Machine Learning Specialization](https://www.coursera.org/specializations/machine-learning-introduction) (audit free) | Andrew Ng's structured ML foundations | 4 to 19 |
| [scikit-learn user guide](https://scikit-learn.org/stable/user_guide.html) | Every classical algorithm and evaluation tool | 4 to 20 |
| [Interpretable Machine Learning](https://christophm.github.io/interpretable-ml-book/) | Explainability methods | 13 |
| [Forecasting: Principles and Practice](https://otexts.com/fpp3/) | Time series forecasting | 21, 22 |
| [Neural Networks: Zero to Hero](https://karpathy.ai/zero-to-hero.html) | Backprop to GPT, built from scratch | 23, 33 |
| [Dive into Deep Learning](https://d2l.ai/) | Deep learning with math and code | 24 to 29 |
| [PyTorch tutorials](https://pytorch.org/tutorials/) | PyTorch basics to GANs | 24 to 30 |
| [Practical Deep Learning for Coders](https://course.fast.ai/) | Top-down deep learning and deployment | 26 |
| [Hugging Face Learn](https://huggingface.co/learn) | Transformers, LLMs, diffusion, agents, deep RL | 31 to 38 |
| [Reinforcement Learning: An Introduction](http://incompleteideas.net/book/the-book-2nd.html) | RL theory, free book | 37, 38 |
| [Made With ML](https://madewithml.com/) | Production ML and MLOps | 39 to 47 |
| [MLOps Zoomcamp](https://github.com/DataTalksClub/mlops-zoomcamp) | Tracking, orchestration, deployment, monitoring | 39 to 47 |

Optional paid book worth buying around week 4: *Hands-On Machine Learning with Scikit-Learn and PyTorch* by Aurélien Géron, which follows almost the same order as this path.
