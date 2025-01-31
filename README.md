This is an analysis of social biases in RAG (retrieval-augmented generation), as well as an
implementation of a technique to mitigate that bias. RAG is a technique for implementing text search via large language model embeddings.

For evaluation, the code here uses the GrepBiasIR dataset ("Gender REPresentation Bias for Information Retrieval")
to evaluate gender bias, as well as search quality.

The mitigation technique shows a 30% reduction in bias when removing 45% of dimensions.
This is commensurate with industry standard practice of dropping 50% of dimensions for the purpose of cost savings.

This repository contains a copy of the original GrepBiasIR dataset, as well as precomputed embeddings for all the documents in that dataset, using various embedding models.
To use the precomputed embeddings, you will need to uncompress embeddings.zip.
To regenerate the embeddings for yourself, you will need to provide your API keys for various embedding providers (e.g. OpenAI and Google)
