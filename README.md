# Fin 101 Chatbot

This chatbot, implemented using the Gemini API, is designed to train on documents in PDF format. It processes the content of the textbooks and allows users to query the material. The chatbot leverages advanced NLP techniques to provide accurate, context-aware responses to any question related to the documents, making it a valuable tool for  professionals seeking quick and reliable information from the text.

## Installation

create the project directory
```shell
mkdir appian_ai_challenge
```

move to the project directory
```shell
cd appian_ai_challenge
```

clone the repository
```shell
git clone https://github.com/Saminathan-77/appian_ai_challenge.git
```

## Usage

Get the GEMINI API KEY from the ```https://ai.google.dev/gemini-api/docs/api-key```.

Add the API KEY to the ```.env``` file.
```shell
API_KEY = ''
```

Install the dependencies from the requirements.txt file
```shell
pip install -r requirements.txt
````

Run the Streamlit application
```shell
streamlit run app.py
```

### Phase 1: Core Chatbot Functionalities

  - **Data Extraction and Cleaning**:
      Extracted relevant text, images, and tables from the PDFs using the Gemini API. Data was cleaned by removing irrelevant sections and stored in a database for fast access.

  - **Increasing Text Retrieval Accuracy**:
      The Gemini API was used to enhance the chatbot's ability to retrieve accurate and relevant text based on user queries. Text was indexed for fast retrieval.

  - **Support for Probing Questions**:
      When the chatbot is unsure of a query, it asks clarifying questions to improve accuracy. This was done by setting confidence thresholds in the response.

  - **Retrieval of Relevant Image and Table Content**:
      Images and tables were tagged during data extraction. Relevant visual data is fetched and presented along with the text for user queries.

  - **Latency Optimization**:
      Caching and efficient processing were implemented to reduce response times. Cloud services were used to ensure scalability and quick responses.

### Phase 2: Advanced Chatbot Functionalities

  - **Image-Based Prompts**:
      The chatbot processes image inputs, using the Gemini API to interpret and respond to visual data such as diagrams.

  - **Flowchart Generation for Relevant Queries**:
      The chatbot generates flowcharts to simplify complex processes, enhancing user understanding of the queried concepts.

  - **Table Reconstruction**:
      The chatbot reconstructs tables using data extracted by the Gemini API, ensuring accurate and structured presentation for the user.

  - **Answering Reference Questions at the End of Each Chapter**:
      The chatbot accurately answers reference questions by linking the query to specific sections of the documents, using indexed content.

  - **Final Latency Optimization**:
       Asynchronous processing and additional caching were implemented to handle higher loads and further reduce response times.

## Feedback
If you have any issues, reach out to us.
