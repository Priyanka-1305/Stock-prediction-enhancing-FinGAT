# Stock-prediction-enhancing-FinGAT

In this project, I have tried to enhance the FinGAT (Financial Graph Attention Network) model. I have used LSTMs for getting temporal learning, GAT for inter and intra sector relations and optimized loss functions. SmoothLoss and BSE with logitloss to minimize the losses during training. By doing so I have managed to outperform FinGAT in some metrics such as MRR (Mean Reciprocal Rank), IRR (Investment Return Ratio), movement accuracy and MAE (Mean Absolute Error).

Metrics obtained from this model:

MAE: 0.0194, MSE: 0.0009 amnd movement accuracy: 51%

| **k** | **MRR@k** | **Precision** | **IRR@k** |
|:-----:|:---------:|:-------------:|:---------:|
| 5     | 0.0866    | 0.2000         | 0.1536    |
| 10    | 0.0671    | 0.3000          | 0.2188    |
| 20    | 0.0594    | 0.2500          | 0.3973    |


To run this project, download all the files from this repository. Open FINAL_STOCK_PREDICTiIONS_RL.ipynb in google colab and run it. When asked, upload the csv file ind_nifty500list_filtered_final.csv and run it.

To run Graph.ipynb, upload in on google colab and run it. Upload the ind_nifty500list_filtered_final.csv file first. Mount updated_sentiment_scores.csv on your drive and run the code further. This file will give all graph visualizations.

The graph file was made trying to integrate sentiments with the stock data, but it was not being generated correctly and was giving poorer results. Hence, sentiments were not used in the main model.
