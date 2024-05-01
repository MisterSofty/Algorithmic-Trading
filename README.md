# Algorithmic-Trading

## Baseline Performance

Parameters:

- short window: `4`
- long window: `100`
- training dataset: `3 months`

Results:

### SVM Classifier Report


![Screenshot 2024-05-01 113534](https://github.com/MisterSofty/Algorithmic-Trading/assets/152457412/2ef2a121-d87f-4282-ad2b-b1d095277c72)


### Cummulative Returns


![Screenshot 2024-05-01 113550](https://github.com/MisterSofty/Algorithmic-Trading/assets/152457412/8208133f-e3df-4709-bfee-33204b8303f7)


The model displays a `55%` accuracy rate as outlined in the `SVM` Classifier Report, while showing `96%` of buy opportunities and `4%` of sell opportunities. The `Strategy Returns` have outperformed the `Actual Returns` for this particular model.

## Adjustment 1


Parameters:

- short window: `4`
- long window: `100`
- training dataset: `8 months`

Results:

### SVM Classifier Report


![Screenshot 2024-05-01 122235](https://github.com/MisterSofty/Algorithmic-Trading/assets/152457412/a298924a-b5ca-4441-83ab-8d5ad9c88631)


### Cummulative Returns


![Screenshot 2024-05-01 120403](https://github.com/MisterSofty/Algorithmic-Trading/assets/152457412/d8970a2a-e0c3-4ca2-bd81-583c961bccfa)

The model displays a `54%` accuracy rate as outlined in the `SVM` Classifier Report, while showing `83%` of buy opportunities and `16%` of sell opportunities. The `Strategy Returns` had a period of severe underperformance compared to the `Actual Returns`, but quickly regained positive performance.


## Adjustment 2


Parameters:
- short window: `4`
- long window: `200`
- training dataset: `3 months`

Results:

### SVM Classifier Report


![Screenshot 2024-05-01 122040](https://github.com/MisterSofty/Algorithmic-Trading/assets/152457412/5116ede7-848a-4663-88d1-75e1e614d119)


### Cummulative Returns


![Screenshot 2024-05-01 122051](https://github.com/MisterSofty/Algorithmic-Trading/assets/152457412/f3bdc5e7-4b16-4017-9748-ac9228525f63)


The model displays a `47%` accuracy rate as outlined in the `SVM` Classifier Report, while showing `16%` of buy opportunities and `85%` of sell opportunities. The `Strategy Returns` are extremely volatile, overperforming and underperforming randomly.

## Evaluation Report

Using `Logistic Regression`

Results:

### Cummulative Returns

![Screenshot 2024-05-01 122356](https://github.com/MisterSofty/Algorithmic-Trading/assets/152457412/4aa5cedf-f6ca-41d7-8ef2-68d5f438fce3)


The `Logistic Regression` model produced some confusing results.  The model started to underperform both `Actual Returns` and `Strategy Returns`, but quickly balanced both.  Still a drastic reverse in trend towards the end suggests the `Logistic Regression` model may not be the best model to use in this case.
