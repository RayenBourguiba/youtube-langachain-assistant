# YouTube LangChain Assistant

This project is a Streamlit-based assistant that answers questions about YouTube videos using their transcripts. It leverages LangChain, OpenAI models, and vector databases (FAISS) to process and query video content.

## 🔧 Features

- Extracts transcripts from YouTube videos
- Splits transcripts into manageable chunks
- Creates a searchable vector database using FAISS
- Uses OpenAI's `gpt-3.5-turbo-instruct` for answering questions
- Streamlit interface for easy interaction

## 🧰 Technologies Used

- Python
- Streamlit
- LangChain
- OpenAI API
- FAISS
- `langchain_community` and `langchain_openai`
- dotenv for managing API keys

## 🚀 How to Run

1. **Clone the repository**
    ```bash
    git clone https://github.com/yourusername/youtube-langchain-assistant.git
    cd youtube-langchain-assistant
    ```

2. **Set up a virtual environment**
    ```bash
    python -m venv .venv
    source .venv/bin/activate  # On Windows: .venv\\Scripts\\activate
    ```

3. **Install dependencies**
    ```bash
    pip install -r requirements.txt
    ```

4. **Set your OpenAI API key**

    Create a `.env` file:
    ```
    OPENAI_API_KEY=your_openai_key_here
    ```

5. **Run the app**
    ```bash
    streamlit run main.py
    ```

## 📌 Notes

- `gpt-3.5-turbo-instruct` is used because `text-davinci-003` has been deprecated.
- Make sure the YouTube video you are analyzing has subtitles or transcripts available.

## 📝 License

This project is open source and free to use under the MIT License.
