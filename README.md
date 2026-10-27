<<<<<<< HEAD
***# RAG Experiments: Chunking and Retrieval***



***This repository documents my hands-on experiments with Retrieval-Augmented Generation (RAG) using Python, LangChain, Chroma, and OpenAI models.***



***The goal is to understand how document preparation and retrieval choices influence the context provided to a language model and the answers it generates.***



***## Experiments***



***### Experiment A: Character Text Splitting***

***Explore document chunking with `CharacterTextSplitter`, inspect chunk sizes, and examine how the resulting chunks can be used in a RAG pipeline.***



***### Experiment B: Recursive Text Splitting***

***Use `RecursiveCharacterTextSplitter` to compare chunk statistics, store embeddings in Chroma, and inspect retrieved passages.***



***### Retrieval: Similarity Search and MMR***

***Explore similarity-based retrieval and Maximum Marginal Relevance (MMR), testing different relevance-diversity settings.***



***## Experiment B: Key Observations***



***- `CharacterTextSplitter` produced 21 chunks, while `RecursiveCharacterTextSplitter` produced 19.***

***- The recursive splitter produced a higher average chunk length in this experiment.***

***- Different MMR settings changed the passages retrieved.***

***- In the observed answer comparison, the character-splitter pipeline produced a more complete answer, while the recursive pipeline was more cautious about missing information.***



***These observations come from a limited experiment and do not establish that one splitting method is universally better.***



***## Tools and Technologies***



***- Python***

***- LangChain***

***- Chroma***

***- OpenAI embeddings and chat models***

***- Jupyter Notebook***



***## Limitations***



***The answer comparison used one main test question. Retrieval and response quality were assessed qualitatively rather than with formal evaluation metrics.***



***## Future Improvements***



***- Test more questions and document types.***

***- Evaluate retrieval relevance systematically.***

***- Compare answer quality using consistent evaluation criteria.***

***- Explore alternative chunking and retrieval strategies.***



***## Running the Experiments***



***1. Create and activate a Python environment.***

***2. Install the dependencies listed in `requirements.txt`.***

***3. Configure your OpenAI API key as a local environment variable.***

***4. Open the notebooks in Jupyter and run the cells in order.***



***Do not commit API keys, private documents, local environment files, or other sensitive data to the repository.***



***This repository is part of my ongoing journey in AI engineering, documenting what I test, what I observe, and what I learn.***
