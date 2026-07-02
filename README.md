# Airline Customer Satisfaction - Decision Tree Classification

## Project Summary
This project builds an optimized Decision Tree classifier to predict
airline passenger satisfaction using survey data. GridSearchCV was
used to tune hyperparameters and prevent overfitting. The model
achieves an F1-Score of 0.946 and identifies Inflight Entertainment
as the strongest driver of customer satisfaction.

## How to Run
1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Upload `Invistico_Airline.csv` when prompted
4. Run all cells in `decision_tree_airline.ipynb`

## Dataset
- Source: Invistico Airline Passenger Survey
- Size: 129,880 passengers, 22 features
- Target: satisfaction (satisfied/dissatisfied)
- Missing values: 393 in Arrival Delay — dropped

## Best Hyperparameters (GridSearchCV)
| Parameter | Value |
|-----------|-------|
| max_depth | 15 |
| min_samples_split | 10 |
| min_samples_leaf | 1 |

## Model Performance
| Metric | Score |
|--------|-------|
| F1-Score | 0.946 |

## Top 5 Feature Importances
| Feature | Importance |
|---------|------------|
| Inflight entertainment | 0.440 |
| Seat comfort | 0.198 |
| Ease of Online booking | 0.071 |
| Customer Type | 0.047 |
| Gate location | 0.026 |

## Decision Tree vs Logistic Regression
| Criteria | Decision Tree | Logistic Regression |
|----------|--------------|---------------------|
| Interpretability | HIGH | MEDIUM |
| Non-linear relationships | Yes | No |
| Business actionability | Easy to explain | Needs expertise |
| F1-Score | 0.946 | Lower |

## Business Recommendations
1. Invest in inflight entertainment upgrades — strongest driver
2. Improve seat comfort — second most important factor
3. Streamline online booking experience
4. Use decision tree pathways for staff training
5. Deploy model for real-time passenger satisfaction screening

## Environment Setup
pip install -r requirements.txt

## Files
- decision_tree_airline.ipynb — Main analysis notebook
- README.md — Project documentation
- requirements.txt — Dependencies
