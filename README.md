# ATELIER2
# NLP Techniques for Text Processing: A Brief Report
This report summarizes the exploration of various NLP techniques for text processing, encompassing rule-based approaches, word embeddings, and dimensionality reduction.
## Part 1: Rule-Based NLP and Regex
This section focused on extracting information from a sample text using regular expressions and rule-based NLP to generate a bill from a user-provided description of purchased items.
### Process:
1. Stop Word Removal: Words like "bought," "for," and "each" were removed to simplify processing.
2. Item Extraction: Regex identified item names (e.g., "Samsung smartphones," "Hamburger").
3. Quantity and Price Extraction: Separate regexes extracted quantities (e.g., "three") and prices (e.g., "150").
4. Data Cleaning and Calculation: Quantities were converted to integers, prices to floats, and total prices calculated.
5. Bill Generation: A Pandas DataFrame organized the information, and tabulate presented the bill in a table.
This demonstrated the effectiveness of regex and rule-based NLP for straightforward information extraction tasks.

## Part 2: Word Embeddings
This section explored various word embedding techniques to represent words as numerical vectors, capturing semantic relationships. The dataset from Lab 1 was utilized.

### Implemented Techniques:
1. One-Hot Encoding: Creates binary vectors representing word presence/absence in the vocabulary.
2. Bag-of-Words (BoW): Counts word occurrences, creating vectors representing word frequency.
3. TF-IDF: Extends BoW by considering word importance based on document and corpus frequency.
4. Word2Vec (CBOW & Skip-Gram): Learns word embeddings by predicting word context or vice versa.
5. GloVe: Utilizes word co-occurrence statistics to learn word representations.
6. FastText: Considers subword information for handling rare or out-of-vocabulary words.
   
### Visualization and Evaluation:
T-SNE visualized high-dimensional word embeddings in 2D space, aiding in understanding word clustering and relationships based on different embedding techniques.

### Conclusion:
Word embedding techniques offer powerful tools for representing words and capturing semantic relationships. Choosing the best technique depends on the specific task and dataset. While one-hot encoding and BoW are simple, TF-IDF is better for document retrieval. Word2Vec, GloVe, and FastText provide more nuanced representations for various NLP applications.
## Learning Outcomes
This lab provided valuable experience in applying NLP techniques like regex, rule-based approaches, and word embedding models. It highlighted their strengths and limitations and emphasized the importance of choosing the right method for specific tasks. Further exploration is encouraged for deeper understanding and improved NLP skills.
