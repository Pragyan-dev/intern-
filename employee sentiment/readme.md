# Employee Sentiment Analysis – Summary

## Overview
This project analyzes employee sentiment using a Hugging Face transformer model (`cardiffnlp/twitter-roberta-base-sentiment`) on email messages from 2010–2011. The analysis includes:  
- Sentiment classification  
- Employee scoring  
- Flight risk identification  
- Predictive modeling  

## Key Findings

### Top Three Positive Employees (January 2010)
1. **Eric Bass** (`eric.bass@enron.com`): Score 3  
2. **Patti Thompson** (`patti.thompson@enron.com`): Score 3  
3. **Don Baughman** (`don.baughman@enron.com`): Score 2  

### Top Three Negative Employees (January 2010)
1. **Sally Beck** (`sally.beck@enron.com`): Score –1  
2. **Bobette Riner** (`bobette.riner@ipgdirect.com`): Score 0  
3. **John Arnold** (`john.arnold@enron.com`): Score 0  

### Employees Flagged as Flight Risks  
*(Average sentiment score < –0.5 in any rolling 30-day window)*  
- `bobette.riner@ipgdirect.com`  
- `don.baughman@enron.com`  
- `john.arnold@enron.com`  
- `sally.beck@enron.com`  

## Insights
- **Sentiment Distribution:**  
  - Neutral: 1485  
  - Positive: 558  
  - Negative: 148  
  Indicates a generally stable workforce with a slight positive lean.

- **Monthly Trends:**  
  Neutral messages dominate each month (85–90 entries), with consistent proportions over time.

- **Flight-Risk Signals:**  
  Flagged employees show similar negative‐sentiment levels (~0.9), suggesting comparable risk profiles.

- **Predictive Model Performance:**  
  - MSE: 0.000  
  - R²: 1.000  
  The perfect fit likely indicates overfitting—further validation is needed.


