# Content-Summarization
This project utilizes LangChain and the Groq API to create a Streamlit application that summarizes content from YouTube videos or websites. It demonstrates the power of large language models in processing and condensing information from various online sources.
# Features
- Summarize content from YouTube videos or any website URL
- User-friendly interface built with Streamlit
- Integration with Groq API for advanced language processing
- Flexible input options for users

# How It Works
- User Input: Users provide a Groq API key and a URL (YouTube video or website) through the Streamlit interface.
- Content Loading:
    - For YouTube videos: Uses YoutubeLoader to extract video transcripts.
    - For websites: Uses UnstructuredURLLoader to fetch and parse webpage content.
- Summarization:
    - Utilizes the Gemma-7b-It model via the Groq API.
    - Applies a custom prompt template to generate a 300-word summary.
- Output: Displays the generated summary to the user.
# Implementation Details
- The app uses LangChain's load_summarize_chain with a "stuff" chain type for summarization.
- Custom prompt template focuses on providing a concise 300-word summary.
- Error handling and input validation ensure a smooth user experience.
# Setup and Running
- Install dependencies
 ```bash
pip install -r requirments.txt
```
- Set up a Groq API key
- Run the application
 ```bash
stremlit run app.py
```
# Technologies Used
- Python
- Streamlit
- LangChain
- Groq API
- YouTube Transcript API
- UnstructuredURLLoader
