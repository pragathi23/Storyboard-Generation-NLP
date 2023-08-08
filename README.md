# Storyboard-Generation-NLP
## Introduction
Our NLP-based PowerPoint Generator revolutionizes the process of creating presentations and
storyboards from lengthy PDF documents. By leveraging Natural Language Processing (NLP)
techniques, this innovative system drastically reduces the time and effort required for these tasks.
The generator extracts key information from the PDFs, ensuring accurate comprehension of
concepts and data points. It then generates a comprehensive storyboard as the foundation for
visually appealing PowerPoint slides. Our solution streamlines the creation process, saving
valuable time and effort. The presentations and storyboards maintain consistency and clarity
throughout, delivering impactful results.
In summary, our NLP-based PowerPoint Generator offers an efficient approach to transform PDF
documents into compelling presentations. With automated information extraction and voice over
capabilities, users can create engaging slides with ease.

![image](https://github.com/pragathi23/Storyboard-Genearation-NLP/assets/102874384/dedfc95c-5385-442c-aae9-6c79f2c5866e)


## Scope of the Project
The scope of this project encompasses the development of an advanced NLP-based PowerPoint
Generator with a focus on providing a user-friendly interface and efficient generation of visually
appealing presentations. The system will be capable of effectively processing both long and short
documents to produce high-quality PowerPoint slides.
The core functionalities of the PowerPoint Generator include automated extraction and
summarization of key information which will also provide a seamless and intuitive user interface,
ensuring ease of use for individuals with varying levels of technical expertise.
As a future enhancement, the project aims to incorporate interactive storyboards, enabling features
such as quizzing and integration of videos, to enhance audience engagement and interactivity. This
expansion will further elevate the overall user experience and create a more dynamic and
immersive presentation environment.
The development process has been organized and structured, encompassing essential stages such
as requirement analysis, sequence diagram creation, state diagram design, and high-level system
design. This systematic approach ensures a well-defined and organized development path,
facilitating efficient implementation and robust system performance.
The project emphasizes delivering a visually appealing user interface and efficient performance,
ensuring the generated PowerPoint presentations are of high quality. By incorporating user
feedback and iterative development practices, the system will undergo continuous improvement to
meet user requirements and enhance user satisfaction.

## Problem statement
The manual process of converting lengthy PDF documents into PowerPoint presentations is timeconsuming and inefficient, lacking automated extraction and synthesis of key information. This
results in presentations that often fail to engage the audience effectively. To overcome these
challenges, our project aims to develop an NLP-based PPT generator that can analyze PDF
documents, extract essential points, and generate visually captivating slides with relevant images.
By optimizing the extraction algorithm, improving the user interface, and conducting
comprehensive testing, our goal is to significantly reduce the time and effort required to create
compelling presentations, empowering users with a powerful tool to enhance communication and
productivity in various fields.

## Design
### High Level Design
The high-level design of the application involves a structured workflow that includes document
input, text preprocessing, extraction of text in JSON format for seamless pipelining into
PowerPoint slides, classification of text into headings, subheadings, and summary points ensuring
a well-organized content structure, text summarization, and generation of the PowerPoint
presentation. Users upload documents as input, followed by text preprocessing for optimization.
The extracted text is transformed into JSON format to facilitate smooth data handling. The
summarized text is generated using advanced techniques, condensing it into concise key points.
Finally, the application generates visually appealing PowerPoint slides. This high-level design
guarantees a systematic and efficient approach to create compelling presentations with structured
content hierarchy.

![image](https://github.com/pragathi23/Storyboard-Genearation-NLP/assets/102874384/5432bf6d-3f1d-4dac-af84-362262d5482f)


## Detailed Design
The user will login through the interactive user interface after which they can upload the pdf to be
summarized, which is then taken for summarization. The output is then pipelined for PPT generation
which is visually appealing.
![image](https://github.com/pragathi23/Storyboard-Genearation-NLP/assets/102874384/8c9e3375-94cd-4df8-8839-72cf2ced12f4)


![image](https://github.com/pragathi23/Storyboard-Genearation-NLP/assets/102874384/ccefa111-99e0-4447-8a1d-865062947b26)


## Sequence Diagram
As shown in the diagram user is an actor interacting with the system. As shown in the design After
opening the webpage, user has to login. After successful login, the user uploads the document , the
model is used to summarize the text which gives the output in JSON to generate the PPT which is
then returned to the user.

![image](https://github.com/pragathi23/Storyboard-Genearation-NLP/assets/102874384/4a572713-0f6b-4bde-8c8e-cae6db53329f)

## Use Case Diagram
As shown above there are two actors interacting with the system, one is the user and the other one
is the System. The user has use-cases like authentication, login and logout. The user and system is
responsible for the document management. The system will process the input document by
preprocessing, ppt generation, and summarization which can be accessed by the user.

![image](https://github.com/pragathi23/Storyboard-Genearation-NLP/assets/102874384/2c1e9047-99be-4ae4-aecb-7a2904eda06c)


## Implementation
### Proposed methodology
The project uses a combination of methodologies and techniques for text summarization. The
original text in the input document undergoes several preprocessing steps, including
tokenization, stop word removal, and other text cleaning techniques. Once pre-processed, the text
is classified into headings, subheadings, and content.
Techniques used in the project:
1. Tokenization: The original text is divided into individual tokens, usually words or
subwords, to facilitate further processing and analysis.
2. Stop Word Removal: Commonly used words with little semantic meaning, such as "the,"
"is," and "and," are removed to reduce noise in the text and improve the quality of the
summary.
3. Text Cleaning: Various techniques are employed to clean the text, including removing
punctuation, converting text to lowercase, and handling special characters or symbols.
4. Headings and Subheadings Extraction: The document is analysed to identify headings
and subheadings based on formatting, such as font size, style, or indentation.
5. Sentence Importance Scoring: Techniques like TF-IDF (Term Frequency-Inverse
Document Frequency) or LDA (Latent Dirichlet Allocation) are used to assign
importance scores to sentences based on their relevance to the main topics or themes in
the document.
6. Postprocessing: The obtained summary content is further processed to refine its
readability and coherence. This may include capitalizing the first letter of each sentence,
adding appropriate punctuation, and ensuring proper formatting.
7. JSON Format: The final summarized content is structured in JSON (JavaScript Object
Notation) format, which is a lightweight data interchange format widely used for data
representation and communication.
8. PPT Pipeline: The summarized content in JSON format is then pipelined into a
PowerPoint (PPT) presentation, where it can be used to generate slides or populate
existing slide templates with the summarized information.
9. Latent Semantic Analysis (LSA) Methodology:
● LSA is a technique used for text summarization that involves analyzing the
relationships between words and documents in a high-dimensional space.
● It starts by constructing a term-document matrix that represents the frequency of
terms in the document collection.
● Next, the matrix is factorized using singular value decomposition (SVD), which
reduces the dimensionality of the matrix and identifies the underlying latent
semantic structure.
● By representing the text in a lower-dimensional space, LSA can capture the main
topics and relationships between words and sentences.
● The importance of sentences is determined based on their similarity to the main
topics, and the most important sentences are selected to form the summary.

## Algorithm used for implementation
LSA (Latent Semantic Analysis) is a mathematical technique used for text analysis and
information retrieval. It aims to capture the underlying semantic structure of a document
collection by analysing the relationships between words and documents. LSA represents text in a
lower-dimensional space, allowing for efficient processing and summarization. Here is a detailed
explanation of LSA:
1. Building the Term-Document Matrix:
● The first step in LSA is to construct a term-document matrix that represents the
frequency of terms in the document collection.
● The matrix has rows corresponding to terms and columns corresponding to
documents.
● Each entry in the matrix represents the frequency or weight of a term in a
document.
● Various weighting schemes can be used, such as term frequency (TF), inverse
document frequency (IDF), or TF-IDF.
2. Singular Value Decomposition (SVD):
● After constructing the term-document matrix, LSA applies Singular Value
Decomposition (SVD) to factorize the matrix.
● SVD breaks down the matrix into three separate matrices: U, Σ, and V^T.
● U represents the left singular vectors, which capture the relationships between
terms.
● Σ is a diagonal matrix containing singular values, which indicate the importance
of each dimension.
● V^T represents the right singular vectors, which capture the relationships between
documents.
3. Dimensionality Reduction:
● The dimensionality of the term-document matrix is typically very high, which
makes processing and analysis computationally expensive.
● To reduce the dimensionality, LSA truncates the singular values and
corresponding singular vectors.
● By keeping only the top k singular values and their associated vectors, the matrix
is transformed into a lower-dimensional representation.
● The choice of k determines the level of dimensionality reduction and the amount
of information retained.
4. Sentence/Document Similarity Calculation:
● Once the dimensionality is reduced, LSA calculates the similarity between
sentences or documents based on their vector representations.
● The similarity between two vectors can be computed using various metrics, such
as cosine similarity.
● Cosine similarity measures the cosine of the angle between two vectors, providing
a value between -1 and 1. Higher values indicate greater similarity.
5. Sentence Importance Scoring:
● LSA assigns importance scores to sentences based on their similarity to the main
topics or themes in the document collection.
● One common approach is to calculate the sentence importance score as the sum of
the similarities between the sentence vector and the main topic vectors.
● The main topic vectors can be obtained by averaging the vectors of the top-k
documents that are most representative of each topic.
6. Sentence Selection for Summarization:
● After scoring the sentences, LSA selects the most important sentences to form the
summary.
● The number of sentences selected depends on the desired length of the summary.
● The selected sentences should capture the main ideas and themes of the document
while maintaining coherence and readability.

## LSA STATISTICS:

![image](https://github.com/pragathi23/Storyboard-Genearation-NLP/assets/102874384/4838bfa1-364f-4bb7-b3bd-23f47a302b8e)

## Conclusion and Future Work
In this project, we implemented Latent Semantic Analysis (LSA) for text summarization and
successfully generated summaries from input documents. We employed techniques such as
tokenization, stop word removal, and classification into headings, subheadings, and content. LSA
proved to be an effective method for summarization, extracting important sentences based on
semantic similarity. The generated summaries were post-processed to obtain concise and
informative content in JSON format, which was then pipelined into PowerPoint presentations
(PPT).
The project also provides an interactive user interface (UI) that is intuitive and user-friendly. The
UI would allow users to easily upload documents, customize summarization settings, and navigate
through the generated PPTs. Attention will be given to user feedback and iterative improvements
to ensure a seamless and satisfying user experience.
Future Work: To enhance the accuracy of the summarization process, several avenues can be
explored. Firstly, developing multiple templates for PPTs or storyboards would allow for greater
customization and presentation options. The selection of templates could be based on a machine
learning model trained on user preferences or the nature of the content. Additionally, incorporating
web scraping techniques to gather topic-related images and integrating them into the PPTs would
enhance visual appeal and engagement.
Furthermore, an exciting future enhancement would be the addition of interactive quizzes and
questions based on the content. This would transform the PPTs into interactive learning
experiences, providing an opportunity for users to test their knowledge and reinforce key concepts.
Additionally, incorporating voice-over notes would provide an additional layer of explanation and
improve accessibility for users.
In conclusion, the project successfully implemented LSA for text summarization and generated
informative summaries. Future work includes enhancing accuracy through template selection,
integrating web scraping for relevant images, incorporating interactive quizzes, adding voice-over
notes, and improving the interactive UI. These advancements will create a more engaging and
comprehensive summarization tool that can effectively convey information and facilitate
interactive learning experiences.
