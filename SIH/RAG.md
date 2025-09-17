### Efficient Document Processing for LLM Interaction

#### Overview
Instead of feeding entire documents directly to a language model (LLM), we implement a more efficient pipeline that extracts and processes relevant text segments before LLM interaction. This approach addresses the inefficiency of raw document processing and ensures LLM receives only the most relevant information.

#### Pipeline Process
1. **Document Preprocessing:**
   - Convert documents to text (PDF to text extraction)
   - **Chunking:** Divide the text into meaningful segments (e.g., paragraphs or sentences)
   - Convert text chunks into vector representations (embeddings)
1. **Vector Database Storage:**
   - Store the vector embeddings in a vector database for efficient retrieval.

#### Retrieval Process
1. **User Query Processing:**
   - Convert the user's query into a vector representation.
2. **Vector Matching:**
   - Perform a similarity search in the vector database to find the top 3-5 most relevant text chunks.
   - Vector matching compares the query vector with document vectors using a similarity metric (e.g., cosine similarity).
3. **Result Return:**
   - Return the top matching text segments to the LLM for natural language response generation.

#### Vector Matching Explained
Vector matching leverages the geometric properties of vector spaces to find semantically similar text segments.
- **Embedding:** Convert text segments and queries into high-dimensional vectors using an embedding model (e.g., BERT, Sentence-BERT).
- **Similarity Calculation:**
  - **Cosine Similarity:** Measures the angle between vectors; higher values indicate greater similarity.
  - **Euclidean Distance:** Measures the straight-line distance between vectors in the space; shorter distances indicate greater similarity.
$$ \text{cosine similarity} = \frac{A \cdot B}{\|A\| \|B\|} $$

  Where $A$ and $B$ are vectors, $A \cdot B$ is the dot product, and $\|A\|$ and $\|B\|$ are the magnitudes (Euclidean norms) of vectors $A$ and $B$, respectively.
- **Retrieval:** Retrieve top-k most similar vectors based on the chosen similarity metric.