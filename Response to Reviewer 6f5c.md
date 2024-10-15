# Response to Reviewer 6f5c

$\textbf{Q3:}$ More related works should be cited in Section Introduction.

$\textbf{A3:}$ Thank you for your advice. We appreciate your suggestion to include more related works. We will expand our Introduction section to provide a more comprehensive overview of existing approaches in e-commerce representation learning. We would like to emphasize that **RelationExpert is the first work to propose a general e-commerce self-supervised representation learning framework** that combines RelationEmbed: a hypergraph foundation model designed to capture complex group-wise relationships in e-commerce data. and TaskReport: an interpretability-driven module that generates explanatory reports for downstream tasks.

While the works you mentioned [1,3,4,5] make valuable contributions, they primarily focus on graph-based approaches rather than hypergraph-based methods that can capture higher-order relationships. Our hypergraph approach allows us to model the complex, multi-entity interactions common in e-commerce scenarios more effectively. Regarding this work [2], while it does propose a hierarchical hyperedge embedding-based representation learning for group recommendation, it focuses on social media platforms like Yelp and Douban. In contrast, our work is specifically tailored to e-commerce environments, considering the unique high-order relationships among products, customers, and merchants in online marketplaces. RelationExpert's novelty lies in its comprehensive approach to e-commerce representation learning, combining hypergraph-based modeling with interpretable outputs, which addresses key challenges in the field that previous works have not fully explored.


[1] Cao, Da, et al. "Attentive group recommendation." The 41st International ACM SIGIR conference on research & development in information retrieval. 2018. 

[2] Guo, Lei, et al. "Hierarchical hyperedge embedding-based representation learning for group recommendation." ACM Transactions on Information Systems (TOIS) 40.1 (2021): 1-27. 

[3] Wang, Wen, et al. "Group-aware long-and short-term graph representation learning for sequential group recommendation." Proceedings of the 43rd international ACM SIGIR conference on research and development in information retrieval. 2020. 

[4] Cao, Da, et al. "Social-enhanced attentive group recommendation." IEEE Transactions on Knowledge and Data Engineering 33.3 (2019): 1195-1209. 

[5] Chen, Chong, et al. "Social attentional memory network: Modeling aspect-and friend-level differences in recommendation." Proceedings of the twelfth ACM international conference on web search and data mining. 2019.



$\textbf{Q4:}$ Additional hyper-parameter tuning experiments.

$\textbf{A4:}$ Thanks for your valuable suggestion. Yes, we have used grid search to search the optimal hyper-parameters. Due to space limits, we did not put these experimental results in the manuscript. For clarity, here we list two sets of experiments to investigate the influence of the trade off hyper-parameter $\lambda_1$ and $\lambda_2$, and  the hyper-parameters of learning rate. From table 1, we find out the model performance on **both tasks are relatively robust on different sets of ($\lambda_1$, $\lambda_2$)** and it gains the best performance on (1.0, 1.0). Besides, in table 2, we find out **the model performance on both tasks is still relatively robust**. It gains the best performance when the learning rate is 0.1 while it has relatively large variances. So the learning rate of 0.001 can be a good trade-off value of learning rate.

 $\textbf{Table 1}:$ Performance comparison of different trade-off hyper-parameters  ($\lambda_1$, $\lambda_2$) on abusive group detection task on M1 market (Task 1) and AP performance of product-customer link prediction task on M1 market (Task 2).


| Task 1 - (0.1, 0.1) | Task 1 - (0.5, 0.1) | Task 1 - (0.5, 1.0) | Task 1 - (1.0, 1.0) | Task 2 - (0.1, 0.1) | Task 2 - (0.5, 0.1) | Task 2 - (0.5, 1.0) | Task 2 - (1.0, 1.0) |
|---------------------|---------------------|---------------------|---------------------|---------------------|---------------------|---------------------|---------------------|
| 53.14 ± 4.95 | 52.73 ± 4.89 | 52.89 ± 4.95 | **53.53 ± 4.92** | 60.01 ± 3.15 | 59.71 ± 3.45 | 59.87 ± 3.11 | **60.12 ± 3.14** |


 $\textbf{Table 2}:$ Performance comparison of different learning rate  on abusive group detection task on M2 market (Task 1) and AP performance of  product-customer link prediction task on M2 market (Task 2).

| Task 1 - 0.1 | Task 1 - 0.01 | Task 1 - 0.001 | Task 1 - 0.0001 | Task 2 - 0.1 | Task 2 - 0.01 | Task 2 - 0.001 | Task 2 - 0.0001 |
|---------------------|---------------------|---------------------|---------------------|---------------------|---------------------|---------------------|---------------------|
| **48.28 ± 4.11** | 48.05 ± 3.42| 48.17 ± 3.97 | 47.95 ± 3.72 |**56.32 ± 3.78** | 56.08 ± 3.25 | 56.14 ± 3.14 | 55.94 ± 3.05 | 




To conclude, we sincerely hope our responses have adequately addressed your concerns regarding our paper. If you feel that we have sufficiently addressed all of your concerns in this rebuttal, we would be grateful if you would consider revising your score to reflect this. We welcome any further comments or questions you may have, and we thank you for your thorough review and valuable feedback.
