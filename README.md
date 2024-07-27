# mrl_and_binary_embeddings
 combining matryoshka embeddings and binary embeddings for more scalable searches

 
# Details

MRL - Matryoshka Representation Learning is an approach that helps us obtain varying dimensional representations/vectors instead of a fixed dimension vector. This is achieved by diffusing the information in intermediate dimensions rather than diffusing it along the entire dimension.

Adaptive Retrieval is an important process for efficient retrieval of vectors. With MRL (Matryoshka Representation Learning), it is as simple as performing a single forward pass on the neural network, resulting in a collection of representations with different dimensions.

BINARY EMBEDDING - it is a  technique used to reduce the precision of a number to 1 bit i.e b = sign(x)

sign = 1, x >= 0  and 0, x < 0

exmaple : x= 0.3
1 =sign(x)

RERANKING WITH BINARY EMBEDDINGS - these is basically a reranking step where the candidate documents that are retrieved by binary embeddings are reranked.

         Inner_Product(float_query,binary_doc)

Simply put, the dot product of the fp32 query vector and the binary vector of the candidate document indicates how similar the float vector and the binary vector are, or in other words the similarity  between  query(float vector) and candidate document(binary vector). This similarity measure helps in reranking the candidate documents.
         
         

Both of these techniques are independent of each other and can be easily combined for superior storage savings and fast vector processing.



# References

1. **MRL Paper**: [Matryoshka Representation Learning (MRL)](https://arxiv.org/pdf/2205.13147)
2. **MRL Blog**: [Matryoshka Representation Learning (MRL) Blog](https://aniketrege.github.io/blog/2024/mrl/)
3. **Binary Embeddings Blog**: [Embedding Quantization Blog](https://huggingface.co/blog/embedding-quantization)
