# In-depth Analysis on Conversations Dataset

This repository contains a comprehensive analysis of the `OpenLeecher/GPT4-10k` dataset, which consists of conversations on various topics such as coding, debugging, storytelling, and science. The analysis is performed using various natural language processing techniques to uncover insights and patterns in the data.

## Dataset Overview

The dataset is a comprehensive collection of 100 diverse conversations presented in text format. These conversations cover a wide range of topics, including:

- Coding techniques
- Debugging strategies
- Storytelling methods
- Spatial thinking
- Logical thinking
- Scientific fields (chemistry, physics, biology)
- Law

The dataset is available in a CSV file named `train.csv`, with each conversation represented as a series of messages exchanged between participants.
The dataset can be found in **Kaggle**: [Conversations on Coding, Debugging, Storytelling](https://www.kaggle.com/datasets/thedevastator/conversations-on-coding-debugging-storytelling-s/data)

## Analysis Steps

The analysis is documented in a Jupyter Notebook named `analysis_conversations_dataset.ipynb`. The following advanced techniques are used:

1. **Exploratory Data Analysis:** Understanding the structure and basic statistics of the dataset.
2. **Text Preprocessing:** Cleaning and preparing the text data for further analysis.
3. **Sentiment Analysis:**
   - Sentiment analysis using TextBlob.
   - Sentiment analysis using VADER.
4. **Named Entity Recognition (NER):** Identifying named entities in the text to extract important information.
5. **Text Clustering:** Using K-means clustering to group similar conversations and identify common topics within each cluster.
6. **Conversational Dynamics Analysis:** Analyzing the length and distribution of conversations.
7. **Semantic Similarity Analysis:** Measuring the similarity between different conversations using BERT embeddings.

## Summary

This analysis provides valuable insights into the nature and content of the conversations in the dataset. By leveraging advanced natural language processing techniques, we can uncover patterns, emotions, and key topics within the dialogues. These findings can be useful for developing more sophisticated conversational AI systems and for further research in the field of natural language processing.

### Conclusion

This comprehensive analysis explores various aspects of the conversations dataset, revealing important insights and trends. The advanced techniques used in this analysis can serve as a foundation for further research and development in conversational AI and natural language processing.

## How to Use

1. Clone the repository:
    ```sh
    git clone https://github.com/debjit-mandal/conversations-analysis.git
    cd conversations-analysis
    ```

2. Ensure you have the required libraries installed:
    ```sh
    pip install pandas numpy nltk textblob spacy sklearn matplotlib seaborn sentence-transformers transformers
    ```

3. Download the required NLTK and Spacy data:
    ```python
    import nltk
    nltk.download('punkt')
    nltk.download('stopwords')
    nltk.download('vader_lexicon')

    import spacy
    spacy.cli.download('en_core_web_sm')
    ```

4. Open the Jupyter Notebook to explore the analysis:
    ```sh
    jupyter notebook analysis_conversations_dataset.ipynb
    ```

## Acknowledgements

If you use this dataset or the analysis in your research, please credit the original authors:

- Peevski (From Huggingface)
- [Dataset Source](https://huggingface.co/datasets/OpenLeecher/GPT4-10k)

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any improvements or additional analyses.

## License

This project is licensed under the CC0 1.0 Universal (CC0 1.0) - Public Domain Dedication. You can copy, modify, distribute, and perform the work, even for commercial purposes, all without asking permission.