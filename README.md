## Megabundles On-chain Prediction
This notebook demostrates three models that can be used to predict whether Flashbots megabundles will land on-chain based on the block data that contains bundles actually landed on-chain.

Among the three models, one unsupervised learning model is used to find out if there are any features in the block data that might contribute to the outcome of landing on-chain and could be used to predict the same for megabundles; two supervised learning models are used to train the block data in order to predict which megabundles will land on-chain.

The results from these three models are summarised below:

K Means: Using a two clusters K Means model, gas_used, block_net_profit and ssinceblockstart play important roles in the separation of these two clusters.
Gamma Distribution: It predicts with a 90% confidence level that 72% of the blocks is expected to have a megabundle land on-chain. The additional profits that could have been made if these megabundles were included on-chain are 7,751 ETH from block number 14000001 to 14132593.
Logistic Regression: It predicts with a 90% confidence level that 68% of the blocks is expected to have a megabundle land on-chain. The additional profits that could have been made if these megabundles were included on-chain are 7,069 ETH from block number 14000001 to 14132593.
