# 📊 Employee Sentiment Analysis (TextBlob-based)

This project analyzes internal email communications to evaluate employee sentiment using TextBlob. The analysis includes sentiment classification, employee scoring, flight risk identification, and a predictive modeling component.

---

## 🏆 Top 3 Positive and Negative Employees (Overall)

| Rank | Positive Employees              | Score | Negative Employees              | Score |
|------|---------------------------------|-------|----------------------------------|-------|
| 1    | kayne.coulter@enron.com        | 9     | rhonda.denton@enron.com         | 0     |
| 2    | don.baughman@enron.com         | 5     | bobette.riner@ipgdirect.com     | 2     |
| 3    | eric.bass@enron.com            | 5     | johnny.palmer@enron.com         | 2     |

---

## 🚨 Employees Flagged as Flight Risks

These employees had a high frequency of negative messages in a 30-day period:

- bobette.riner@ipgdirect.com (Flagged: 2010-11-17)
- don.baughman@enron.com (Flagged: 2010-03-07)
- eric.bass@enron.com (Flagged: 2010-04-15)
- john.arnold@enron.com (Flagged: 2010-06-18)
- johnny.palmer@enron.com (Flagged: 2010-02-26)
- lydia.delgado@enron.com (Flagged: 2010-11-25)
- patti.thompson@enron.com (Flagged: 2010-05-02)
- rhonda.denton@enron.com (Flagged: 2010-08-28)
- sally.beck@enron.com (Flagged: 2010-07)

---

## 🔍 Key Insights

- Most employee messages show a **positive sentiment**, suggesting a generally optimistic culture.
- **Message length and word count** have a strong positive correlation, but only a weak correlation with sentiment score.
- Sentiment scores fluctuate **monthly**, indicating possible morale trends that align with organizational events.
- A **flight risk detection rule** was developed using a rolling 30-day window for negative message counts.

---

## 📈 Predictive Model Summary

- A **Linear Regression** model was built to predict sentiment scores based on message statistics.
- **Performance:**
  - R² Score: `0.641`
  - MSE: `4.206`

---