# **RAG & LLM with Pathway to Process Financial Reports and Tables**

## **Overview**

This project is for building a system that leverages Retrieval-Augmented Generation (RAG) and large language models (LLMs) to process financial reports and tables. The system integrates structured data (e.g., tables) and unstructured data (e.g., text, images) with Claude Sonet 3.5, using Pathway’s Google Drive Connector and Streamlit for the user interface.


---

## **Key Components and Technologies**

### **1. Pathway Framework**

* **RAG Pipelines:** Pathway’s efficient pipeline framework is used to build scalable workflows for real-time and batch processing of multimodal data.
* **Google Drive Connector:** Handles real-time data ingestion from Google Drive for seamless integration of financial reports.
* **VectorStore/DocumentStore:** Enables instant access and retrieval of relevant data for analysis.

### **2. Claude Sonet 3.5**

* **LLM:** A powerful large language model used for natural language understanding and generation to analyze textual and tabular data.
* **Multimodal Processing:** Handles diverse data formats, enhancing the insights derived from financial reports.

### **3. Streamlit**

* **Frontend:** Provides an interactive user interface for visualizing financial data insights and interacting with the system.

---

## **Folder Structure**

/financial-report-insights

    ├── app.py            # Backend processing script with Pathway pipeline.

    ├── app.yaml          # Pathway configuration for deployment.

    ├── Dockerfile        # Dockerfile for containerization.

    ├── requirements.txt  # Python dependencies.

    ├── credentials.json  # Google Drive credentials.

    ├── streamlit_app.py  # Streamlit frontend for user interaction.

    └── claude_llm.py     # Contains ClaudeSonetLLM class for interacting with Claude Sonet's API.

## **Description of Files**

* **app.py:**
    * Implements the main Pathway pipeline.
    * Connects to Google Drive for ingesting financial reports.
    * Processes structured and unstructured data using RAG and Claude Sonet 3.5.
* **app.yaml:**
    * Contains deployment configurations for running the Pathway pipeline in production or test environments.
* **Dockerfile:**
    * Configures the application’s environment for containerized deployment.
    * Ensures compatibility and portability across systems.
* **requirements.txt:**
    * Specifies Python dependencies, including pathway, streamlit, and other necessary libraries.
* **credentials.json:**
    * Stores authentication credentials for accessing Google Drive.
* **streamlit_app.py:**
    * Builds an interactive frontend using Streamlit.
    * Displays financial insights and enables user input for specific queries.
* **claude_llm.py:**
    * Defines the ClaudeSonetLLM class, encapsulating the interaction logic with Claude Sonet’s API.
    * Supports multimodal data queries and responses.

---

## **Conclusion**

By combining Pathway’s real-time processing capabilities with the Claude Sonet 3.5 LLM, this system enables efficient analysis of multimodal financial data. The use of Streamlit enhances accessibility and usability, providing a comprehensive tool for financial insights.
