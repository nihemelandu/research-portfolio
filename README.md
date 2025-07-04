# Welcome to My Research Portfolio

## Research Statement

My past research focused on identifying and recommending best practices for applying statistical inference in the analysis of recommender system evaluation experiments. The goal was to enhance the reliability of performance metrics by addressing key statistical challenges and improving the accuracy of evaluation results.

Currently, I am exploring causal inference techniques to estimate the true causal effects of recommended items on user behavior. This research aims to refine the reliability of performance metrics in recommender systems by better understanding the causal relationships between recommendations and user interactions.

# 📦 Research Plan: Causal Dynamics Between Customer Behavior and Supply Chain Operations

## 🧭 Overview

This research aims to investigate the **bidirectional relationship** between algorithmic customer interactions and supply chain operations. Specifically, it explores how **digital experiences and demand signals** influence procurement, inventory, and fulfillment—and how those operational realities, in turn, shape **customer experience and satisfaction**.

The end goal is to improve **decision quality** and **operational efficiency** in complex, dynamic supply chain environments using robust causal reasoning and system modeling.

---

## 🎯 Research Objectives

- Determine whether changes in customer behavior **cause** operational impacts, or are merely correlated.
- Evaluate whether improvements in supply chain performance **lead to** measurable gains in customer satisfaction or loyalty.
- Model and simulate feedback loops between demand-side behaviors and supply-side constraints.
- Inform **intervention design** that aligns customer-facing decisions with operational capabilities.

---

## 🧩 Research Scope

### 🔍 Domain Focus

To make this work tractable and actionable, the research will focus on a well-defined domain:

- **Industry selection**: Retail, e-commerce, or manufacturing (TBD)
- **Customer behavior metrics**:
  - Purchasing patterns
  - Complaint or return rates
  - Channel preferences
  - Conversion & churn
- **Operational performance metrics**:
  - Inventory turnover
  - Fulfillment accuracy
  - Delivery time & reliability
  - Flexibility and cost efficiency
- **Significance threshold**:  
  Not all statistically significant effects are **operationally meaningful**—this research will prioritize interventions with **practical impact**.

---

## 🛠️ Methodology

To address the causal questions at the heart of this work, a hybrid approach will be employed, drawing from structural models, quasi-experiments, causal machine learning, and simulation.

---

### 🧠 1. Structural Causal Models (SCM)

SCMs will serve as the **core reasoning framework** for this research:

- **Causal DAGs (Directed Acyclic Graphs)** to explicitly express assumptions
- **Structural Equations** to model data-generating processes
- **do-Calculus** to derive valid interventional estimands
- **Identification analysis**: Determine whether effects of interest can be identified from available data
- **Toolkits**: [`DoWhy`](https://github.com/py-why/dowhy), [`DAGitty`](http://www.dagitty.net/), `causalgraphicalmodels`, `Ananke`

SCMs provide conceptual rigor and clarity in defining what can (and cannot) be learned from observational data.

---

### 🧪 2. Quasi-Experimental Designs

To estimate causal effects from historical or operational data without randomization:

- **Interrupted Time Series (ITS)**
- **Synthetic Control Methods**
- **Stepped-Wedge Rollout Designs**
- **Panel Event Study Designs**
- **Difference-in-Differences (DiD)**
- **Regression Discontinuity / Kink Designs**
- **Propensity Score Matching / Weighting**

These methods leverage **natural experiments, system rollouts, shocks, or thresholds**—common in supply chain and digital environments.

---

### 🤖 3. Causal Machine Learning

To handle high-dimensional data, discover treatment heterogeneity, and support complex modeling:

- **Causal Forests** (e.g., Generalized Random Forests)
- **Double Machine Learning (DML)**
- **Meta-learners**: S-learner, T-learner, X-learner
- **Uplift Modeling** for individual-level intervention targeting

**Toolkits**: `EconML`, `CausalML`, `scikit-uplift`, `DoWhy + sklearn`

These methods enable estimation at **scale**, with interpretability and flexibility.

---

### 🧪 4. Simulation Modeling

Simulation will be used to model dynamics that are hard to capture empirically:

- **System Dynamics Models**: Capture stock-flow relationships and feedback loops (e.g., inventory → lead times → customer abandonment)
- **Agent-Based Models (ABM)**: Represent decision-making by individual customers, suppliers, or fulfillment centers
- **Scenario Testing**: Examine the effects of hypothetical interventions (e.g., algorithmic changes or new delivery policies)

Simulation allows us to **stress-test** causally-informed strategies in synthetic but realistic environments.

---

## 📏 Evaluation Strategy

### 🔬 Simulation Validation

- **Historical backtesting**: Compare simulation outcomes to observed behavior
- **Face validity**: Are dynamics reasonable to domain experts?
- **Sensitivity analysis**: Explore robustness of outcomes to model assumptions

### 📈 Empirical Evaluation

- **Causal identification**: Are estimated effects statistically and practically valid?
- **Operational interpretability**: Do findings align with stakeholder understanding?
- **Counterfactual testing**: Can the models answer "what-if" questions reliably?

---

## 🔄 Future Directions

- Model **algorithmic feedback loops**, e.g., recommender systems affecting demand patterns, which then affect fulfillment capabilities.
- Extend to **omnichannel environments** where customer behavior spans physical and digital touchpoints.
- Explore real-time adaptive decision systems combining causal inference with online learning or reinforcement learning.

---


## Publications

### [Statistical Inference: The Missing Piece of RecSys Experiment Reliability Discourse](https://arxiv.org/abs/2109.06424)
*Discusses how statistical inference is often overlooked in recommender system evaluations and outlines challenges that threaten experimental reliability.*

### [Inference at Scale: Significance Testing for Large Search and Recommendation Experiments](https://arxiv.org/abs/2305.02461)
*Explores how significance tests behave in large-scale experiments, emphasizing the need to consider practical effect sizes alongside p-values.*

### [Multiple Testing for IR and Recommendation System Experiments](https://md.ekstrandom.net/pubs/ecir2024-multiple-testing.pdf)
*Examines the multiple-comparison problem (MCP) in evaluations involving more than two systems, which can lead to inflated false discoveries. This study extends the investigation to recommendation system evaluations and explores procedures that control the False Discovery Rate (FDR).*

### [Candidate Set Sampling for Evaluating Top-N Recommendation](https://arxiv.org/pdf/2309.11723)
*Analyzes how candidate set selection strategies interact with popularity bias and affect the accuracy of evaluation metrics in top-N recommendation tasks.*

---

## Future Research Goals

### Causal Inference in Recommender Systems
I aim to deepen my exploration of **causal inference methods** to estimate the true causal effects of recommended items on user behavior. This work will focus on refining the evaluation metrics of recommender systems by understanding the direct and indirect effects of recommendations on user actions, ultimately leading to more accurate and reliable performance measurements.

### Supply Chain Decision-Making Under Uncertainty
In the future, I plan to apply **simulation modeling**, **decision optimization**, and **causal inference methods** to improve decision-making processes in **supply chain operations under uncertainty**. This research will seek to optimize supply chain decision-making, particularly in dynamic environments, and help enhance the operational efficiency of supply chains faced with uncertainty in demand, supply, and logistics.

### Integrating Machine Learning with Causal Inference
A significant goal of my future work is to integrate **machine learning** with **causal inference** methods to develop more robust, data-driven solutions for both recommender systems and supply chain applications. This will involve designing novel frameworks that combine the power of ML models with causal reasoning to provide deeper insights and better decision-making capabilities in real-world systems.

---

## Applied Projects 🛠️

### **Forecasting for Predictive Modeling**  
**Skills**: Feature engineering, data preprocessing, time series analysis, machine learning (XGBoost, Random Forest), Python (Pandas, Scikit-learn)

Developed a forecasting model to predict future outcomes such as customer behavior, sales, or demand, using historical data. This project demonstrates the ability to handle **time-dependent or feature-driven data** and leverage various forecasting techniques to make accurate predictions.

Key steps:
- **Feature Engineering**: Processed raw data to extract meaningful features that can help improve prediction accuracy.
- **Modeling**: Applied forecasting models (e.g., time series models for sequential data or machine learning models for feature-driven forecasting).
- **Evaluation**: Used relevant performance metrics (e.g., RMSE, MAPE) to assess model effectiveness and ensure reliable predictions.

---

### **Causal Inference for Estimating Treatment Effects**  
**Skills**: Causal analysis, statistical modeling, hypothesis testing, Python (Pandas, Statsmodels)

Applied **causal inference** methods to identify and estimate the causal relationships between variables in a dataset. The goal was to understand how changes in one variable directly affect another, providing insights for better decision-making and intervention planning.

Key steps:
- **Data Exploration**: Identified key variables and potential causal relationships.
- **Causal Modeling**: Applied causal inference techniques (e.g., regression discontinuity, propensity score matching, difference-in-differences) to estimate treatment effects or causal impacts.
- **Evaluation**: Validated the causal conclusions using statistical tests and sensitivity analysis.

---

### **Discrete-Event Simulation of Bank Client Service**  
**Skills**: Simulation modeling, Python (SimPy, Matplotlib)

Created a **discrete-event simulation** for a bank’s client service system, where clients arrive at the bank, use ATM or teller services, and leave. The simulation tracks key performance indicators, such as **resource utilization** (e.g., ATM and teller usage), and provides insights into the efficiency of the service system.

Key steps:
- **Simulation Design**: Modeled client arrival, ATM, and teller service processes as discrete events.
- **Performance Metrics**: Analyzed key metrics such as **wait times**, **resource utilization**, and **service throughput**.
- **Modeling and Analysis**: Used Python (SimPy) for modeling the system and visualized the results using Matplotlib.

---


## About Me

I hold a PhD with a research focus on statistical and causal inference methods for evaluating recommender systems. My work focuses on improving the reliability of recommender system evaluations by addressing statistical challenges such as significance testing, multiple comparisons, and evaluation bias. I am currently expanding into decision-making under uncertainty in supply chain operations, using simulation, optimization, and causal inference techniques.

---

Feel free to explore the individual papers for more in-depth discussions of the methodologies and findings. For any questions or further details on my work, feel free to reach out!






<!--
<h1>Ngozi Ihemelandu <br/>Data Scientist <br/> <a href="https://www.linkedin.com/in/nihemelandu/">linkedin</a>
</h1> 
<h2>📺Data Analytics Techniques and Methodologies:</h2>

  - <b>[Descriptive Analytics](https://github.com/nihemelandu/Descriptive-Analytics.git) </b>
  - <b>[Causal Inference](https://github.com/nihemelandu/Causal-Inference.git) </b>
  - <b>[Predictive Analytics](https://github.com/nihemelandu/Predictive-Analytics.git) </b>
  - <b>[Prescriptive Analytics](https://github.com/nihemelandu/Prescriptive-Analytics.git) </b>
  - [Praciting DS & Algos in Python](https://github.com/joshmadakor1/Algorithms-Practice)
<h2>📺Independent Projects:</h2>
<h2>👨‍💻 Research Projects:</h2>

- <b>[Pairwise Significance Testing for Recommendation Experiments](https://github.com/Ngozi-Ihemelandu/Prj2-Pairwise-Testing)</b>
- <b>[Multiple Testing for Recommendation System Experiments](https://github.com/Ngozi-Ihemelandu/Prj3-Multiple-Testing)</b>


<h2>📺 Exploratory Data Analysis</h2>
  - <b>[With Python](https://github.com/nihemelandu/EDA_PYTHON.git) </b>

  
<h2> 🤳 Connect with me:</h2>

**nihemelandu/nihemelandu** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
-->
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
