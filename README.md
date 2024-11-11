# Word2Vec Analysis on BPJS Data

## Project Description

This project implements the Word2Vec model to analyze text data related to BPJS (Badan Penyelenggara Jaminan Sosial) in Indonesia. The objective is to explore semantic relationships between words in the context of health services and social insurance. The analysis includes finding synonyms, filling in blanks in sentences, and performing analogical reasoning.

## Structure of the Repository

```
Word2Vec_BPJS_Analysis/
│
├── data/
│ ├── data_ready_final_v2.xlsx # Dataset used for analysis
│ ├── idwiki_word2vec_300.model # Pre-trained Word2Vec model
│
├── reports/
│ ├── Tugas_Word2Vec_PBA_KEL_1_BPJS.pdf # Detailed report of the analysis
│
├── notebooks/
│ ├── Word2Vec_Final_Week_11.ipynb # Jupyter Notebook containing code and analysis
│
└── README.md # Project description 
```

# Word2Vec Analysis on BPJS Data

## Results Summary

The experiments conducted using the Word2Vec model yielded several important insights:

### 1. Data Quality Matters
The performance of Word2Vec is highly dependent on the quantity and quality of data. Models trained from scratch performed worse than those pre-trained on larger datasets, such as *text8* or *idwiki_word2vec_300.model*. Even a well-trained model can yield suboptimal results if relevant context is missing from the training data.

### 2. Impact of Data Cleaning
After updating the model with cleaned BPJS data, the results improved significantly. The cleaned data allowed for better semantic understanding, leading to more accurate predictions during synonym searches and analogical reasoning tasks.

### 3. Synonym Analysis
The synonyms identified for key terms related to BPJS demonstrated meaningful associations. For example, "sehat" (healthy) was closely related to "bpjs" and "jkn" (Jaminan Kesehatan Nasional), indicating a strong contextual relationship within health services.

### 4. Filling in Blanks
The model successfully filled in blanks in sentences with contextually appropriate words, such as "penanganan" (handling) for medical expenses, showcasing its ability to understand contextual meanings.

### 5. Analogy Performance
The model demonstrated its capability in performing analogical reasoning with reasonable accuracy, successfully identifying relationships between terms like "sehat," "sakit," and "bpjs." However, some predictions were less relevant, indicating areas for further improvement.

## Conclusion
Overall, this project illustrates that the Word2Vec model can effectively capture semantic relationships within the context of health services and social insurance when trained with high-quality, relevant data. Further fine-tuning and experimentation with different parameters may enhance model performance even more.

