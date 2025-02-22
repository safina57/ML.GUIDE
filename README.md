
# ML Guide

ML Guide is a multi-LLM agent system designed to assist users with their machine learning problems. It takes in a user's ML problem and dataset, performs exploratory data analysis (EDA), extracts relevant research papers from arXiv, searches the web for similar problems using JiraAI Reader tool, and generates code for the best model to solve the user's problem. This system leverages CrewAI for multi-LLM agent orchestration, Streamlit for the web application, Sweetviz for EDA, Jira AI Reader for research extraction, and Serper API for web scraping.

## Features

- **Exploratory Data Analysis (EDA)**: Automatically performs an initial EDA using Sweetviz to give users insights into their dataset.
- **Research Paper Extraction**: Extracts relevant research papers from arXiv to provide users with the latest developments in the field.
- **Web Scraping for Similar Problems**: Uses JiraAI Reader and Serper API to search the web for similar machine learning problems and solutions.
- **Model Code Generation**: Generates code for the best machine learning model tailored to the user's problem using multi-LLM agents managed by CrewAI.

## Installation

To get started with ML Guide, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/achrefbenammar404/AINS-ML.Guide.git
   cd AINS-ML.Guide
   ```

2. **Set up a virtual environment** (optional but recommended):
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install the required packages**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables**:
   Create a `.env` file in the root directory and add the following variables:
   ```ini
   GROQ_API_KEY = "your_Groq_api_key_here"
   JINA_API_KEY = "your_jina_api_key_here"
   SERPER_API_KEY = "your_serper_api_key_here"
   ```

## Usage

To run the ML Guide application, execute the following command:
```bash
streamlit run src/app.py
```

This will start the Streamlit web application. Open the provided URL in your web browser to interact with the ML Guide interface.

### Steps to Use ML Guide:

1. **Input Problem and Dataset**: Upload your dataset and describe your machine learning problem.
2. **Exploratory Data Analysis**: View the automatic EDA report generated by Sweetviz.
3. **Research Extraction**: Review the relevant research papers extracted from arXiv.
4. **Web Search**: Examine similar problems and solutions found on the web.
5. **Model Generation**: Get the code for the best model to solve your problem, generated by the multi-LLM agents.


# ML.Guide
