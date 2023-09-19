**Glossary of Notations - Reommendation Systems**

L = The original user-item interaction matrix

L<sub>ij</sub> = Likelihood of i<sup>th</sup> user matching j<sup>th</sup> with item in the user-item interaction matrix

L<sub>i</sub> = The average of observed entries in row i of the user-item interaction matrix

n<sub>i</sub> = The number of observed entries in row of the user-item interaction matrix

L<sub>j</sub> = The average of observed entries in column j of the user-item interaction matrix

n<sub>j</sub> = The number of observed entries in column j of the user-item interaction matrix

x<sub>i</sub> = Features of the i<sup>th</sup> user

y<sub>j</sub> = Features of the j<sup>th</sup> item

M = The matrix where each column is a unique word and each row is a document and the entries represent the frequency of the j<sup>th</sup> word appearing in the i<sup>th</sup> document


U = A user embedding matrix 𝑈 ∈ 𝑅<sup>𝑛×𝑑</sup> , where row i is the embedding for user i denoted by 𝑢<sub>𝑖</sub>

𝑆 = The sigma matrix; a diagonal matrix with shape 𝑟 × 𝑟, where r is the rank / number of latent features

𝑉<sup>𝑇</sup> = An item embedding matrix  𝑉 ∈ 𝑅<sup>𝑚×𝑑</sup> , where row j is the embedding for item  𝑗 denoted by 𝑣<sub>𝑗</sub>

r = The rank / number of latent features𝑟

𝑠<sub>𝑘</sub> = 𝑘<sup>𝑡ℎ</sup> value of sigma matrix 𝑆

𝑢<sub>i𝑘</sub> = The value in the i<sup>th</sup> row and the k<sup>th</sup> column of the matrix 𝑈

𝑣<sub>𝑗𝑘</sub> = The value in the j<sup>th</sup> row and the k<sup>th</sup> column of the matrix 𝑉<sup>𝑇</sup>

$\hat{p}$ = The fraction of observed entities

X = An matrix𝑚 × 𝑛

X<sub>ij</sub>= The i<sup>th</sup> row and the j<sup>th</sup> column of matrix X


𝑓<sub>𝑜𝑏𝑠</sub>(𝑥<sub>𝑖</sub>, 𝑦<sub>𝑗</sub>) = A mathematical function/model learned to make predictions using the observed features of users and items

𝑓<sub>𝑙𝑎𝑡𝑒𝑛𝑡</sub>(𝑢<sub>𝑖</sub>, 𝑣<sub>𝑗<sub>) = A mathematical function/model learned to make predictions using the latent features of users and items

𝐿<sup>𝑜𝑏𝑠</sup> = The matrix of values predicted by the function𝑓<sup>𝑜𝑏𝑠</sup>

𝐿<sup>𝑜𝑏𝑠</sup> <sub>ij</sub> = Predicted value at i<sup>th</sup> row and the j<sup>th</sup> column of 𝐿<sup>𝑜𝑏𝑠</sup>

𝐿<sup>diff</sup> <sub>ij</sub> = Difference between the i<sup>th</sup> row and the j<sup>th</sup> column of matrix 𝐿 and the predicted matrix 𝐿<sup>𝑜𝑏𝑠</sup>

𝐿<sup>𝑀𝐸</sup> = Resultant matrix of matrix estimation on the matrix 𝐿<sup>𝑑𝑖𝑓𝑓</sup>

$\hat{L}$<sub>ij</sub>= Combined estimate value of the i<sup>th</sup> row and the j<sup>th</sup> column of  𝐿<sup>𝑜𝑏𝑠</sup> and 𝐿<sup>𝑀𝐸</sup>

𝐿<sub>ij</sub(t) = Value of thei<sup>th</sup>  row and the j<sup>th</sup> column at time of matrix 𝐿

𝑢<sub>𝑖</sub>(𝑡)<sup>𝑇</sup> = The  𝑖<sup>𝑡ℎ</sup> latent feature at time 𝑡 of matrix 𝑈

𝑢<sub>𝑖</sub>(𝑡)<sup>𝑇</sup>  = Transpose of the 𝑖<sup>𝑡ℎ</sup> latent feature at time  𝑡 of matrix 𝑈

𝑣<sub>𝑗</sub>(𝑡) = The j<sup>𝑡ℎ</sup> latent feature at time of matrix 𝑉

𝑋 = The time Series data

𝑋(𝑡) = Time Series data at a given time 𝑡

𝑇 = The time of the last instance of the time series data

𝑅<sup>𝑑</sup> = Real numbers in the 𝑑-dimensional space

𝑃= The page matrix

𝑃<sub>𝑖𝑗</sub> = The entry at the i<sup>𝑡ℎ</sup> row and the j<sup>𝑡ℎ</sup> column of the matrix 𝑃

(𝑇 + 1 𝑚𝑜𝑑 𝐿) = The remainder after diving 𝑇 + 1 by 𝐿

𝑍 = Concatenation of page matrices for all users and items across time 𝑡

$\hat{𝑍}$= Result of performing matrix estimation over the matrix 𝑍 

𝑘 = Number of measurements

$\hat{𝐿}$<sub>𝑖𝑗</sub>(𝑡) = Predicted value of the i<sup>𝑡ℎ</sup> row and the j<sup>𝑡ℎ</sup> column at time 𝑡

𝑓(𝑢<sub>𝑖</sub>(𝑡), 𝑣<sub>𝑗</sub>(𝑡))= A mathematical function/model learned with inputs as thei<sup>𝑡ℎ</sup> latent feature of users at time and j<sup>𝑡ℎ</sup> latent feature of items at time 𝑡

𝐿<sub>𝑖𝑗𝑘</sub>(𝑡) = Likelihood of the i<sup>𝑡ℎ</sup> user matching with the j<sup>𝑡ℎ</sup> item for a given measurement 𝑘 at some time 𝑡

𝑓<sup>𝑘</sup><sub>𝑜𝑏𝑠</sub> (𝑥<sub>𝑖</sub>, 𝑦<sub>𝑗</sub>) = A mathematical function/model learned using the observed users and items features for a given measurement 𝑘

𝑓<sup>𝑘 </sup><sub>𝑙𝑎𝑡𝑒𝑛𝑡</sub>(𝑢<sub>𝑖</sub>(𝑡), 𝑣<sub>𝑗</sub>(𝑡)) = A mathematical function/model learned over the latent features of users and items for a given time and a given measurement𝑡 𝑘

𝑍<sup>𝑘</sup> = Stacked Page matrices for measurements 𝑘

$\hat{𝐿}$<sub>𝑖𝑗𝑘</sub>(𝑡) = Predicted likelihood of the i<sup>𝑡ℎ</sup> user matching with the j<sup>𝑡ℎ</sup> item in a user-item interaction matrix for a given measurement at a given time𝑘 𝑡

𝐿<sup>𝑑𝑖𝑓𝑓</sup><sub>𝑖𝑗𝑘</sub>(𝑡)= Result of matrix estimation on 𝑍<sup>𝑘</sup>

𝐿<sup>𝑜𝑏𝑠</sup><sub>𝑖𝑗𝑘</sub> = Predicted likelihood of the i<sup>𝑡ℎ</sup> user matching with the j<sup>𝑡ℎ</sup> item in a user-item interaction matrix for a given measurement 𝑘



