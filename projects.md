[Back to Home](https://madelinejmeyers.github.io/) | [Back to Portfolio](https://madelinejmeyers.github.io/ePortfolio/)

# Technical Projects

A collection of my work in software engineering, data analytics, and artificial intelligence, showcasing how my technical skills translate into production-ready software solutions.

---

## Offline Document Intelligence Engine
*   **Technologies:** Python, LangChain, Ollama (Llama 3 / Mistral), Document Parsers (PDF, TXT, DOCX), Vector Embeddings, RAG Pipeline

Developed a privacy-first, offline Document Intelligence Engine enabling users to perform semantic search and question-answering over local documents. 
*   **Local Inference:** Utilized Ollama to run large language models locally, ensuring strict data privacy with zero external API dependencies.
*   **RAG Architecture:** Built retrieval-augmented generation pipelines using LangChain to manage document loading, recursive character chunking, embedding generation, and vector retrieval.
*   **Source Citations:** Configured custom prompt templates and search chains that return precise paragraph citations and contextual answers from loaded files.

---

## [Full-Stack Web Dashboard](https://github.com/MadelineJMeyers/CS-340-Portfolio-Project-Flask-Fork)
*   **Technologies:** React.js, Flask, Node.js, MongoDB, JavaScript, Python, Plotly, CSS3

Engineered a responsive, full-stack analytics application from the ground up, re-architecting a legacy single-file dashboard into a modular, production-ready system.
*   **Modern Frontend:** Developed a React.js client interface with reusable components for interactive filtering, coordinate mapping, and data visualizations.
*   **RESTful Backend:** Created a modular Flask API in Python that acts as a secure intermediary between the client interface and the database.
*   **Scalability:** Leveraged Node.js package management and modular MVC architecture, making the application easier to scale, deploy, and maintain.

For a detailed walkthrough of the re-architecture, see the [Full-Stack Re-engineering Narrative](Narratives.md#artifact-three-narrative).

---

## [Interactive Dashboard Prototype](https://github.com/MadelineJMeyers/CS-340-Portfolio-Project-Enhanced)
*   **Technologies:** JupyterDash, Python, MongoDB, PyMongo, Geopandas, Leaflet, Plotly Dash

Developed an interactive dashboard prototype to search and filter database records, adding visualizations (pie charts, histograms) and coordinate-based mapping.
*   **Query Optimization:** Implemented compound indexing in MongoDB following Equality-Sort-Range (ESR) guidelines, reducing complex filter search times significantly.
*   **Security Integration:** Built a user authentication gateway to restrict dashboard access to authorized users and locked down database queries to predefined parameters.
*   **Custom Filtering:** Wrote query logic employing logical operators (and/or) to streamline animal rescue data analysis by criteria such as age, gender, and training status.

For details on the security and database optimizations, see the narratives for [Software Design & Security](Narratives.md#artifact-one-narrative) and [Database Performance](Narratives.md#artifact-two-narrative).

---

## [Client-Server CRUD Engine](https://github.com/MadelineJMeyers/CS-340-Portfolio-Project)
*   **Technologies:** Python, MongoDB, PyMongo API, Jupyter Notebook

Created the core Python CRUD (Create, Read, Update, Delete) engine that serves as the data access layer for all versions of the dashboard.
*   **Encapsulation:** Wrote reusable database interface methods that encapsulate complex raw queries, ensuring consistent data validation.
*   **Error Handling:** Integrated robust try-except validation blocks for database connection and manipulation operations.

### Walkthrough & Code Design Review
I recorded a code walkthrough video explaining the architecture and design of this data-access layer:

[![Code Design Review on YouTube](https://img.youtube.com/vi/rAu6ldN3Db8/maxresdefault.jpg)](https://www.youtube.com/watch?v=rAu6ldN3Db8)

---

You can view more of my work on my [GitHub profile](https://github.com/MadelineJMeyers).

[GitHub](https://github.com) icon by [Icons8](https://icons8.com)
