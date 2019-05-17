# Detection-of-Embeddings-on-Aircraft-Fault-Messages


Vector representation concept proves its success in  solving many real-world problems from a variety of applications.
In this project, we built a novel vector representation model for avionics system for two types of fault messages called MERIT. This new model aims to identify the relationship between the flight deck effects (FDEs) and the maintenance messages (MMSGs) through calculating the embedding co-occurrence matrix between them within a predefined flight leg window.
The  vector space embeddings representation of MERIT is able to differentiate between the strong and weak relationship between messages. Moreover, we benefit from the negative sampling method to incorporate the weak relationship between the FDEs and MMSGs from different subsystems (chapters) in assessing this relationship precisely. We called the developed MERIT with specialized negative sampling approach subsystem-wise MERIT.Both developed models can be used as descriptive and predictive tasks based on the flight leg window used (one and three,respectively). 
The main advantage of the proposed latent aircraft system model (MERIT) is that it needs to be trained only once and can be easily queried using any similarity measurements between the embedding vectors, which means it is more feasible and computationally efficient than traditional machine learning algorithm, where it necessitates building a different model each time for every target FDE. We tested both models on a real Boeing dataset and the experimental results demonstrate the effectiveness of the proposed model in exhibiting the embedded relationships between fault messages and extracting the most relevant predictors.

Word2Vec
Word vectors are simply vectors of numbers that represent the meaning of a word. For now, that’s not very clear but, we’ll come back to it in a bit. It is useful, first of all to consider why word vectors are considered such a leap forward from traditional representations of words.Word vectors represent words as multidimensional continuous floating point numbers where semantically similar words are mapped to proximate points in geometric space. In simpler terms, a word vector is a row of real valued numbers (as opposed to dummy numbers) where each point captures a dimension of the word’s meaning and where semantically similar words have similar vectors.

We can add and subtract vectors — the canonical example here is showing that by using word vectors we can determine that:
king - man + woman = queen
In other words, we can subtract one meaning from the word vector for king (i.e. maleness), add another meaning (femaleness), and show that this new word vector (king — man + woman) maps most closely to the word vector for queen.

In the Word2Vec model, the objective is to compute conditional probabilities of the form P(w|c), where w is a word and c is the context, or P(c|w). In the analysis of text, the context (c) is often the set of words surrounding w.

 In the analysis of text, the context (c) is often the set of words surrounding w. In our proposed framework, the MERIT model, the words can be FDEs and the context can be MMSGs, or vice-versa.
 
 This is a research project which has already been done before . I'll be trying different algorithms to improve the accuracy. The accuracy obtained using Logistic Regression is nearly 10%. But using Google's word2vec it is improved to more than 60%
