# Phishing Email Detection Without Provided Labels

This project detects phishing and spam emails in a competition dataset that came without labels. Our two-person team combined URL rules with an RNN/LSTM/GRU voting model, reached 0.64 accuracy, and advanced to the semifinal round.

## What made the problem interesting

The dataset included email addresses, subjects, and content, but no answer labels. Before training a model, we first had to research the problem and create a way to label the data ourselves.

## Approach

We separated the emails into two paths:

1. **Emails with URLs:** use rule-based phishing website features based on Mohammad et al. (2015).
2. **Emails without URLs:** tokenize the text and classify it with a voting model built from RNN, LSTM, and GRU networks.

We also checked the token distributions after tokenization to understand the text before modeling it.

## Result

| Item | Result |
|---|---|
| Competition | 2022 Crossroads Classic Analytics Challenge |
| Teams | 29 |
| Indiana University placement | Top four |
| Stage reached | Semifinal |
| Final accuracy | 0.64 |

## Team

- Andrew Huang
- Shiue-Yuan Chuang

## Project figures

<img src="fig0.png" width="70%" alt="Project figure 1">

<img src="fig1.png" width="70%" alt="Project figure 2">

<img src="fig2.png" width="70%" alt="Project figure 3">
