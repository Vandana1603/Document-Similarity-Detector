# Document-Similarity-Detector

This project provides a web-based interface to analyze the textual similarity between multiple documents. Users can upload text files and choose between two powerful methods for similarity calculation: TF-IDF (Term Frequency-Inverse Document Frequency) and Sentence-BERT embeddings. The tool then presents a cosine similarity matrix and highlights the most similar document pairs based on a user-defined threshold.

Features
Document Upload: Easily upload multiple text files (.txt) for analysis.
Two Similarity Methods: Choose between:
TF-IDF: A classical statistical method reflecting the importance of a word in a document relative to a corpus.
Sentence-BERT: Utilizes pre-trained transformer models to generate dense vector embeddings for sentences, capturing semantic meaning.
Cosine Similarity: Quantifies the textual similarity between documents using the cosine of the angle between their vector representations.
Interactive Interface: Powered by Gradio, offering a user-friendly experience.
Similarity Matrix: View a comprehensive matrix showing the similarity score between every pair of uploaded documents.

How it Works
Text Preprocessing
Before calculating similarity, the text undergoes basic preprocessing:

Conversion to lowercase.
Removal of non-alphabetic characters.
Tokenization into words.
Removal of common English stop words (e.g., "the", "is", "a").
Stemming using the Porter Stemmer (reducing words to their root form, e.g., "running" to "run").
Similarity Methods
TF-IDF: Documents are transformed into TF-IDF vectors. The cosine similarity is then calculated between these vectors.

Sentence-BERT: The SentenceTransformer model (all-MiniLM-L6-v2) encodes each document into a dense vector embedding. Cosine similarity is then applied to these embeddings.

Output Interpretation
Similarity Score: A value between 0 and 1, where 1 indicates identical content and 0 indicates no similarity.
Highlighting: Red highlighting indicates a similarity score equal to or above the chosen threshold, suggesting potentially very similar content. Green indicates scores below the threshold.

SCREENSHOTS:
<img width="1735" height="773" alt="Screenshot 2026-05-13 190857" src="https://github.com/user-attachments/assets/a558e83e-29a6-4563-a3cf-8b64905c2981" />
<img width="1720" height="775" alt="Screenshot 2026-05-13 190952" src="https://github.com/user-attachments/assets/d142df7e-186b-4f2c-9961-c36c3c384f31" />
<img width="1723" height="773" alt="Screenshot 2026-05-13 191015" src="https://github.com/user-attachments/assets/ecaae6f2-f3a5-45bd-911f-50bd500d9216" />
<img width="1736" height="772" alt="Screenshot 2026-05-13 191115" src="https://github.com/user-attachments/assets/e161e60c-7176-4fdd-bb45-4fbc878eeb30" />

-[VANDANA K]
