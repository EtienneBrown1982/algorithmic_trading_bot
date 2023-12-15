### Create an Evaluation Report

In the previous sections, you updated your `README.md` file with your conclusions. To accomplish this section, you need to add a summary evaluation report at the end of the `README.md` file. For this report, express your final conclusions and analysis. Support your findings by using the PNG images that you created.

# Machine Learning Trading Bot Evaluation Report

![Decorative image.](/Images/14-challenge-image.png)

## Comparative Analysis of SVC Model Returns vs. Actual Returns

# Model Trial 1 Parameters and Summary
Short Window = 4
Long Window = 100
DateOffset = 3 months

Review of F1 Scores:
-1.0 returned a score of 0.07
1.0 returned a score of 0.71

This identifies that the model was better at identifying a buy setup better than a sell setup.

Comparison of cumulative returns can be seen in the graph below and identifies that the SVC model had slightly larger percentage gains than the actual returns with 1.520 vs 1.388 being the respective returns.

![SMA4-100-3month](/Images/sma4_100_3months.png)

# Model Trial 2 Parameters and Summary
Short Window = 4
Long Window = 100
DateOffset = 12 months

Review of F1 Scores:
-1.0 returned a score of 0.00
1.0 returned a score of 0.72

This identifies that the model was better at identifying a buy setup better than a sell setup. With a 0.00 precision and recall as well for the sell setup.

Comparison of cumulative returns can be seen in the graph below and identifies that the SVC matches the actual returns exactly. This makes sense becuase the model is not able to identify a sell point, so the model would exactly track the actual returns.

![SMA4-100-12month](/Images/sma4_100_12months.png)

# Model Trial 3 Parameters and Summary
Short Window = 9
Long Window = 20
DateOffset = 3 months

Review of F1 Scores:
-1.0 returned a score of 0.00
1.0 returned a score of 0.72

This identifies that the model was better at identifying a buy setup better than a sell setup. with a 0.00 precision and recall as well for the sell setup

Comparison of cumulative returns can be seen in the graph below and identifies that the SVC matches the actual returns exactly. This makes sense becuase the model is not able to identify a sell point, so the model would exactly track the actual returns.

![SMA9-20-3month](/Images/sma9_20_3months.png)

# Model Trial 4 Parameters and Summary
Short Window = 9
Long Window = 20
DateOffset = 12 months

Review of F1 Scores:
-1.0 returned a score of 0.00
1.0 returned a score of 0.72

This identifies that the model was better at identifying a buy setup better than a sell setup. with a 0.00 precision and recall as well for the sell setup

Comparison of cumulative returns can be seen in the graph below and identifies that the SVC matches the actual returns exactly. This makes sense becuase the model is not able to identify a sell point, so the model would exactly track the actual returns.

![SMA9-20-12month](/Images/sma9_20_12months.png)

# Model Trial 5 Parameters and Summary
Short Window = 50
Long Window = 200
DateOffset = 12 months

Review of F1 Scores:
-1.0 returned a score of 0.52
1.0 returned a score of 0.45

This identifies that the model was better at identifying a sell setup better than a buy setup.

Comparison of cumulative returns identifies that the model outperforms the actual returns with returns of 1.702 vs 1.591 respectively.

![SMA50-200-12month](/Images/sma50_200_12months.png)

# Model Trial 6 Parameters and Summary
Short Window = 50
Long Window = 200
DateOffset = 24 months

Review of F1 Scores:
-1.0 returned a score of 0.46
1.0 returned a score of 0.57

This identifies that the model was better at identifying a buy setup better than a sell setup.

Comparison of cumulative returns identifies that the model outperforms the actual returns with returns of 1.834 vs 1.400 respectively.

![SMA50-200-12month](/Images/sma50_200_12months.png)

## AdaBoost Returns vs. Actual Returns

# Model Parameters and Summary
Short Window = 4
Long Window = 100
DateOffset = 3 months

Review of F1 Score:
-1.0 returned a score of 0.13
1.0 returns a score of 0.70

This identife sthat the model was better at identifying a buy setup better than a sell setup.

Comparison of cumulative returns identifies that the model outperforms the actual returns with respective returns of 1.570 vs. 1.388.

## Conclusion

Modifying short and long windows and date offsets with the SVC model can adjust model efficacy and profitability. However, when we compare the initial same SVC model parameters with the AdaBoost model, there appears to be a slight advantage to the AdaBoost model. This can likely be further investigated with adjusted model parameters and further comparative analysis.