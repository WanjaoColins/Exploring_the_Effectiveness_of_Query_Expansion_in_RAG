
![getimg_ai_img-uUTAqN6k5lM1zCiyNZRnC](https://github.com/user-attachments/assets/6008bab1-17d3-40b1-a2a7-4ca704368802)


# Exploring_the_Effectiveness_of_Query_Expansion_in_RAG

This project implements a Retrieval-Augmented Generation (RAG) system focused on exploring the effectiveness of query expansion techniques in enhancing document retrieval. By integrating various machine learning libraries and APIs, this system aims to improve the relevance and accuracy of responses generated by language models when querying external knowledge sources.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Experimental Results](#experimental-results)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Features

- **Integration with OpenAI API**: Leverage the power of OpenAI's language models for generating human-like text.
- **Document Retrieval**: Use ChromaDB for efficient document storage and retrieval.
- **PDF Processing**: Extract text from PDF documents using the `pypdf` library.
- **Community Support**: Built on LangChain and LangChain Community libraries for enhanced functionality.
- **Visualization Tools**: Utilize Matplotlib and Umap for visualizing data and results.

## Installation

To set up the project, you will need to install the required libraries. You can do this by running the following commands in your terminal:

```bash
pip install openai
pip install chromadb
pip install pypdf
pip install langchain
pip install langchain_community
pip install openai==0.28.0
pip install langchain-huggingface
pip install sentence_transformers
pip install umap-learn
pip install matplotlib
pip install tiktoken
```

Ensure you have Python 3.x installed on your machine.

## Experimental Results

Based on experimental results comparing document retrieval with and without query expansion, several key findings were observed:

- The baseline performance using the original query method yielded an average distance of **0.2779**.
  
- When implementing query expansion, results varied across three different expanded queries:
  
  - **Query 1**: Slight improvement with an average distance of **0.2662** (4.2% improvement over baseline).
  
  - **Query 2**: Marginally worse performance with an average distance of **0.2795**.
  
  - **Query 3**: Least effective performance with an average distance of **0.2821**.

These results suggest that query expansion does not consistently improve document retrieval effectiveness in our implementation. While Query 1 showed promise, the other expanded queries led to decreased performance, highlighting challenges in implementing effective query expansion techniques.

Future work could focus on:

- Developing more sophisticated term selection methods for expansion.
  
- Implementing relevance feedback mechanisms.
  
- Exploring different weighting schemes for expanded terms.
  
- Analyzing the relationship between query characteristics and expansion effectiveness.

In summary, while query expansion shows potential for improving document retrieval in specific cases, careful consideration must be given to the expansion methodology to ensure consistent improvements in retrieval performance.

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a pull request.

## License

This project is licensed under the MIT License.

## Acknowledgments

- Thanks to OpenAI for providing powerful APIs that enhance language processing capabilities.
  
- Special thanks to contributors and community members who have provided valuable feedback and support throughout this project.
  
- Acknowledgment of libraries and resources that facilitated development, including LangChain framework and ChromaDB.
