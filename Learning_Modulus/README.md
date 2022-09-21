Several attempts at getting a Neural Network to learn a modulus operation (modulo `N` for a small) number `N`.
More concretely, the learning objective is the following:
Input: A non negative integer in binary format, up to `2 ^ k`, if `k` is the size of the input layer (here usually `k = 30`).
Goal: Classify the input according to its value modulo `N`. The loss function is sparse categorical crossentropy with respect to the ground truth.

None of the attempts showed any sign of success, except using an RNN trained on numbers of varying length. However, this simplifies the problem basically to learning the addition operation modulo `N`, so it is not very surprising.