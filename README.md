# Basket Analysis

The dataset can be accessed at the following link:
https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci/


## Metrics
- **Support**
  - Support measures how frequently an association rule happens in a dataset.

- **Confidence**
  - Confidence measures how strong an association rule is.
  - That is to say, in market basket analysis terms, how likely is a second product to be present in the basket if the first is?
  - Confidence(A→B) = Support(A∪B)/Support(A)×100%
  - Confidence(B→A) = Support(A∪B)/Support(B)×100%

- **Lift**
  - Lift measures how much more likely two items are to be bought together compared to being bought individually at random.
  - Lift(A→B)= Support(A∪B)/Support(A)×Support(B)
  - If Lift = 1, it means there is no association between A and B.
  - If Lift > 1, it indicates that A and B are more likely to be bought together than randomly.
  - If Lift < 1, it suggests that A and B are less likely to be bought together than randomly.

- **Leverage**
  - Leverage measures the difference between the observed frequency of A and B occurring together and the frequency that would be expected if A and B were statistically independent.
  - Leverage(A→B)=Support(A∪B)−(Support(A)×Support(B))
  - Positive leverage indicates that the items appear together more frequently than expected by chance.
  - Zero leverage means the items occur together exactly as expected based on their individual supports.
  - Negative leverage implies the items co-occur less frequently than expected.

- **Conviction**
  - Conviction measures the ratio of the expected frequency that A occurs without B to the frequency that A occurs when B is present.
  - Conviction(A→B)= 1−Support(B)/1−Confidence(A→B)
  - Conviction(B→A)= 1−Support(A)/1−Confidence(B→A)
  - If Conviction = 1, it means that A and B are independent of each other.
  - If Conviction > 1, it suggests that the presence of B has increased the likelihood of A, indicating a strong association.
  - If Conviction < 1, it indicates a negative association between A and B.

- **Zhang’s metric**
  - Measure that looks not only at positive associations but also negative. It can be said, for instance, that buying A makes someone NOT buy B.
  - Value: < 0 if there’s a negative association (dissociation), > 0 if there’s a positive association where -1 and 1 are the extreme values.
