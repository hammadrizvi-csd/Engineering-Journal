# FAIML Unit 2 - Machine Learning Basics and Workflow

---

## 1. Machine Learning

Machine Learning is a subset of Artificial Intelligence that provides systems the ability to automatically learn and improve from experience without being explicitly programmed.

---

### Definitions

* Arthur Samuel (1959):
  Machine Learning is a field of study that gives computers the ability to learn without being explicitly programmed.

* Tom Mitchell (1997):
  A program learns from experience (E) with respect to tasks (T) and performance measure (P) if its performance improves with experience.

---

### Example (Spam Filter)

* Task (T): Classify emails as spam or not
* Experience (E): Labeled emails (spam/non-spam)
* Performance (P): Accuracy of classification

---

### Learning from Data

* Traditional programming → Rules written by humans
* Machine Learning → Learns patterns from data
* Can identify patterns and make decisions with minimal human intervention

---

## 2. Brief History of Machine Learning

* 1950s–1960s: Arthur Samuel created checkers program
* 1970s–1980s: Focus on pattern recognition (Nearest Neighbor)
* 1990s: Shift from rule-based to data-driven approaches
* Modern Era: Deep Learning and Big Data revolution

---

## 3. Machine Learning and Big Data

* ML depends on large datasets
* Big Data characteristics:

  * Volume (large data)
  * Variety (different types)
  * Velocity (fast data flow)

More data generally leads to better predictions.

---

## 4. Types of Analytics

---

### Descriptive Analytics (Hindsight)

* Focus: What happened?
* Uses historical data
* Tools: Reports, dashboards

---

### Predictive Analytics (Foresight)

* Focus: What will happen?
* Uses ML models and statistics
* Techniques: Regression, Decision Trees, Neural Networks

---

## 5. AI vs ML vs Statistics

* AI: Broad field of making machines intelligent
* ML: Subset of AI that learns from data
* Statistics: Mathematical study of data

👉 Difference:

* ML focuses on prediction accuracy
* Statistics focuses on interpretability

---

## 6. Types of Machine Learning

---

### 1. Supervised Learning

* Uses labeled data
* Input + correct output given

#### Process:

* Model learns mapping function
* Predicts output for new data

---

#### Types:

##### Classification

* Output: Discrete (Yes/No, Cat/Dog)

##### Regression

* Output: Continuous (Price, Temperature)

---

#### Algorithms:

* Linear Regression
* Decision Tree
* Support Vector Machine (SVM)

---

### 2. Unsupervised Learning

* Uses unlabeled data
* Finds hidden patterns

---

#### Techniques:

##### Clustering

* Group similar data points

##### Association

* Finds relationships between data

---

#### Algorithms:

* K-Means
* Apriori

---

### 3. Semi-Supervised Learning

* Combination of labeled + unlabeled data
* Useful when labeled data is limited

---

### 4. Reinforcement Learning

* Agent learns by interacting with environment

---

#### Key Concepts:

* Reward → positive feedback
* Penalty → negative feedback
* Learns via trial and error

---

#### Examples:

* Self-driving cars
* Game playing AI (AlphaGo)

---

## 7. Classification vs Regression

| Feature    | Classification           | Regression                       |
| ---------- | ------------------------ | -------------------------------- |
| Output     | Categorical              | Continuous                       |
| Goal       | Class prediction         | Value prediction                 |
| Example    | Spam detection           | House price                      |
| Algorithms | Logistic Regression, SVM | Linear Regression, Decision Tree |

---

## 8. Dimensionality Reduction

* Reduces number of features
* Removes redundancy

### Benefits:

* Reduces complexity
* Saves storage
* Improves performance

---

### Technique:

* PCA (Principal Component Analysis)

---

## 9. Neural Networks and Deep Learning

---

### Artificial Neural Network (ANN)

* Inspired by human brain
* Contains:

  * Input layer
  * Hidden layers
  * Output layer

---

### Deep Learning

* Subset of ML using deep neural networks
* Handles large and complex data

---

### Applications:

* Image recognition
* Speech recognition

---

## 10. Training a Machine Learning Model

---

### Step 1: Data Collection

* Collect relevant data
* Sources: databases, sensors, internet

---

### Step 2: Data Preprocessing

* Clean data
* Handle missing values
* Remove duplicates
* Convert data into numeric form

---

### Step 3: Data Splitting

* Training Set (e.g., 80%)
* Testing Set (e.g., 20%)

---

### Step 4: Model Training

* Train model using algorithm
* Adjust parameters

---

### Step 5: Model Selection

* Choose best algorithm
* Based on problem type

---

### Step 6: Evaluation

* Compare predictions with actual results

#### Metrics:

* Accuracy
* Precision
* Recall

---

### Step 7: Deployment

* Use model in real-world
* Improve with tuning

---

## 11. Applications of Machine Learning

---

### Automation

* Replace manual tasks
* Example: Chatbots

---

### Insight Generation

* Discover hidden patterns
* Example: Fraud detection

---

### Personalization

* Customize user experience
* Example: Recommendations

---

### Decision Making

* Data-driven decisions instead of intuition

---

## Summary

* Machine Learning learns from data
* Different types: supervised, unsupervised, reinforcement
* Classification vs regression important
* ML pipeline includes data → training → evaluation → deployment
* Widely used in real-world applications

---
