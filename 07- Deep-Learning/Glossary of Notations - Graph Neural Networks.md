**Glossary of Notations - Graph Neural Networks**

**Transfer Learning:**

X = Input Vector

f(x) = The part of the neural network that we don’t want to train during Transfer Learning

Z = Encoding of the input vector X when it passes the function f(x)

ℎ<sub>pre</sub>(z) = The classifier part of the neural network trained on the **pretext task.** We re-train this

during Transfer Learning

ℎ(z) = The classifier part of the neural network trained on the **target task**

m = The size of the dataset for the pretext task

n = The size of the dataset for the target task

W = Output of the original architecture

Y = Output of the Transfer Learning architecture

x = Original image or anchor

x<sup>+</sup> = Positive sample: derived from the anchor image x

x<sup>−</sup> = Negative sample: not derived from the anchor image x

f(x<sup>+</sup>) = Embedding function applied on positive sample

f(x<sup>−</sup>) = Embedding function applied on negative sample

p<sup>+</sup><sub>x</sub> = Probability that the sample is a positive sample

p<sup>-</sup><sub>x</sub> = Probability that the sample is a negative sample


**Graph Neural Networks:**

ℎ<sub>𝑢</sub> = The feature description / node embedding of node 𝑢

ℎ<sub>𝑢</sub> <sup>(k-1)</sup> = The feature description / node embedding of node 𝑢 in round k − 1

𝑁(𝑣) = Neighboring nodes of node 𝑣

m<sup>(k)</sup><sub>𝑁(𝑣)</sub> = Messages passed to node 𝑣 from all it’s neighbors, i.e., 𝑁(𝑣) in round k

ℎ<sup>(k)</sup><sub>𝑣</sub> = The feature description / node embedding of node 푣 in round 푘

MLP = Multi Layer Perceptron to perform aggregation

MLP<sub>Θ</sub> = MLP used to learn features of each embedding

MLP<sub>ϕ</sub> = MLP used to learn features from the output of adding features of individual embeddings

W<sub>self</sub> = Weight corresponding to the current node while updating the feature description

W<sub>neigh</sub> = Weight corresponding to neighboring nodes while updating the feature description

b = The bias term

