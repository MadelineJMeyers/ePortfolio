[Back to Home](https://madelinejmeyers.github.io/) | [Back to Portfolio Main Page](index.md) | [Back to Projects](projects.md)

# Technical Narratives

Detailed assessments of the design decisions, optimization strategies, and engineering actions behind my key ePortfolio projects.

## Index of Narratives

*   [Software Design & Security Integration](#artifact-one-narrative) — Custom authentication, code refactoring, and UI enhancement.
*   [Database Performance & Optimization](#artifact-two-narrative) — MongoDB query design, ESR compound indexing, and input security.
*   [Full-Stack Re-engineering](#artifact-three-narrative) — Re-architecting a legacy dashboard into a modular React + Flask production application.

---

## <a id="artifact-one-narrative"></a>Software Design & Security Integration

### Background & Challenge
In the initial development phase, the database dashboard lacked secure access controls. Raw CRUD interface modules were exposed directly to the application environment without gating access to client-side data. The goal of this enhancement was to introduce client security and clean up codebase structure for long-term maintenance.

### Implementation & Actions
*   **Authentication Gateway:** Implemented a secure login interface requiring valid user credentials before loading database records or dashboard visualizations. This ensures sensitive search criteria and results are restricted to authorized personnel.
*   **Interface Refactoring:** Integrated a custom export engine allowing users to download query datasets as CSV spreadsheets directly from the UI. Added a "Dark Mode" stylesheet toggle to enhance readability for different screen preferences.
*   **Documentation Standards:** Refactored the underlying Python dashboard script, adding inline documentation and structured header blocks detailing parameter specifications, class methods, and logic flows.

### Outcome & Skills Demonstrated
These enhancements display a strong focus on defensive programming and user-experience engineering. They demonstrate the ability to secure raw backend access scripts while delivering standard business-oriented features (data export, accessibility options).

---

## <a id="artifact-two-narrative"></a>Database Performance & Optimization

### Background & Challenge
To make the dashboard useful for complex target operations, users needed the ability to run compound queries across multiple database fields (such as filtering rescue animals by species, training status, gender, and age). Running unoptimized queries against a growing MongoDB dataset can lead to performance bottlenecks and high latency.

### Implementation & Actions
*   **Query Algorithm Design:** Designed search algorithms utilizing Python query structures. Leveraged nested logical operators and array criteria to build comprehensive filtering options. For instance, used logical OR matching to aggregate search results across multiple genders in a single query, reducing the number of distinct query options.
*   **MongoDB Index Optimization:** Analyzed query patterns and designed compound indexes utilizing MongoDB's **Equality, Sort, Range (ESR)** rules. As shown below, this structures index key configurations starting with exact equality fields, followed by sorting fields, and ending with range criteria.
*   **Input Sanitization:** Ensured the dashboard application only passes predefined parameters to the backend, completely preventing raw input parameters from reaching the query engine to eliminate injection vulnerabilities.

### Index Verification Screenshot
Below is the backend index configuration verified via VS Code and the MongoDB terminal interface:

<img width="975" height="595" alt="MongoDB index verification screenshot" src="https://github.com/user-attachments/assets/9ca24302-fd9b-4295-b835-166f45df3b05" />

### Outcome & Skills Demonstrated
This work demonstrates analytical skills in database optimization and query engine tuning. Applying ESR index configuration significantly reduces search execution time, illustrating an understanding of backend data modeling needed for high-performance software systems.

---

## <a id="artifact-three-narrative"></a>Full-Stack Re-engineering

### Background & Challenge
The original dashboard prototype was implemented as a single-file Jupyter Notebook running JupyterDash. While effective for initial prototyping, a single-file monolithic structure is difficult to scale, test, or deploy within a microservice or cloud-native architecture. 

### Implementation & Actions
*   **MVC Architecture Decoupling:** Re-architected the dashboard into a modern, decoupled Full-Stack web application. Created a React.js frontend for client UI rendering and a modular Flask API backend in Python.
*   **RESTful API Development:** Developed API routes in Flask to process incoming database CRUD requests, returning JSON data payloads to the client. This decoupled the database client drivers from the user interface code.
*   **Modular Component Design:** Broke the monolithic dashboard code into reusable React components (navigation, data tables, charting widgets, map frames). Managed package dependencies securely using Node.js (`npm`).

### Outcome & Skills Demonstrated
This re-engineering showcases the ability to transition a software prototype into a maintainable, modern web application stack. It highlights capabilities in full-stack JavaScript/Python development, modular system design, and the ability to learn and apply new framework ecosystems to deliver value.
