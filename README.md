# Cache Augmented Generation (CAG) Chatbot 🧀

## Overview

The Cache Augmented Generation (CAG) Chatbot is an intelligent conversational system that leverages smart caching and embedding techniques to enhance response times and provide efficient, intelligent interactions. By using semantic similarity matching and intelligent caching strategies, this chatbot can quickly retrieve and generate responses.

## Features 🚀

- **Smart Caching**: Employs a sophisticated caching mechanism to store and retrieve responses
- **Semantic Similarity Matching**: Uses embeddings to find approximate matches in the cache
- **Configurable Parameters**: Allows dynamic configuration of cache size and similarity thresholds
- **Real-time Statistics**: Provides live metrics on cache performance
- **Streamlit Web Interface**: User-friendly web application for interaction

## Prerequisites 📋

Before you begin, ensure you have the following:

- Python 3.8+
- Hugging Face API Key
- Git

## Installation 🔧

1. Clone the repository:
   ```bash
   git clone https://github.com/nastyrunner13/CAG-LLM.git
   cd CAG-LLM
   ```

2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up environment variables:
   - Create a `.env` file in the project root
   - Add your Hugging Face API key:
     ```
     HUGGINGFACE_API_KEY=your_hugging_face_api_key_here
     ```

## Usage 💻

Run the Streamlit application:
```bash
streamlit run app.py
```

### Configurable Options

- **Cache Size**: Adjust the maximum number of cached responses (50-500)
- **Similarity Threshold**: Set the minimum similarity score for cache matching (0.5-1.0)
- **Clear Cache**: Reset the entire cache with a single button click

## How It Works 🧠

1. **Query Submission**: User enters a query
2. **Cache Check**: System checks if an exact match exists in the cache
3. **Semantic Matching**: If no exact match, finds semantically similar queries
4. **LLM Fallback**: If no match found, queries the Mistral-7B language model
5. **Caching**: Successful responses are cached for future use

## Technologies Used 🛠️

- Python
- Streamlit
- Sentence Transformers
- Scikit-learn
- Hugging Face API (Mistral-7B)
- Plotly for visualizations

## Performance Metrics 📊

The application provides real-time insights:
- Cache Hits/Misses
- Cache Size
- Hit/Miss Ratios
- Response Time Trends

## Contributing 🤝

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request
