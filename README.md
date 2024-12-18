# Patent Data Analysis and Visualization

## Overview

This repository contains code, resources, and workflows for analyzing patent data using Python, Apache Spark, AWS, and Microsoft Azure services. The objective of this project is to extract actionable insights and trends from patent datasets to aid intellectual property strategies and business decisions.

---

## Architecture

The workflow follows a **4-phase architecture**:

![image](https://github.com/user-attachments/assets/3025532d-d3aa-4c58-8892-b12441963da5)

1. **Sourcing**: Data is scraped and ingested from major patent repositories such as:
    - Google Patents
    - WIPO
    - USPTO
    - FPO
    - Espacenet

2. **Storage**: Patent data is stored in cloud solutions:
    - Amazon S3
    - Microsoft Azure Blob Storage

3. **ETL (Extract, Transform, Load)**:
    - **Tools Used**: Apache Spark (Azure Databricks) and Delta Lake
    - Data pipelines are built using Azure Data Factory to clean and transform data.
    - The **Medallion Architecture** ensures:
      - Bronze: Raw ingestion
      - Silver: Filtered and clean data
      - Gold: Aggregated and analytics-ready data.

4. **Visualization**: Insights are visualized using:
    - Power BI
    - Matplotlib & Seaborn (Python libraries)

---

## Key Features

- **Web Scraping**: Patent data is extracted using BeautifulSoup and Python scripts.
- **Preprocessing**: 
    - Data cleaning
    - Parsing XML, JSON, CSV, and PDF formats
- **Feature Engineering**: 
    - Keyword extraction
    - Citation network analysis
- **ETL Pipelines**: Scalable data processing with Apache Spark.
- **Visualizations**: Interactive charts for patent trends, keyword frequency, and metrics.

  Count of Patents by Year

  <img width="692" alt="image" src="https://github.com/user-attachments/assets/2d7636f1-7e1d-4e53-8213-7f4436b6258d" />

  Count o Power BI Desktop f inventor by country

  <img width="691" alt="image" src="https://github.com/user-attachments/assets/60ed0cc9-cd3f-4da0-be95-17e48f4c7c69" />
  
  Th Power BI Desktop e development of countries' interest in patenting
  
  <img width="695" alt="image" src="https://github.com/user-attachments/assets/64dd7362-09f3-430c-b0c9-bc04ec7da4e1" />


---

## Project Structure

├── Analysis of Patents on Virus Engineering.pdf   # PDF report on virus engineering patents
├── ETL_PROCESS.ipynb                              # Notebook for the ETL process
├── Interface_DEMO.rar                             # Demo interface (compressed file)
├── Patents_Scraping.ipynb                         # Notebook for web scraping patent data
├── Project_Architecture.png                       # Architecture diagram for the project
├── Project_Presentation.pdf                       # Project presentation file
├── Projet_visualizations.pdf                      # Visualizations and insights in PDF
└── README.md                                      # Project documentation

---

## Installation

### Prerequisites
- Python 3.x
- Apache Spark
- AWS credentials for S3
- Microsoft Azure access

### Steps:
1. **Clone the repository**:
   ```bash
   git clone https://github.com/your_username/patent-analysis.git
   cd patent-analysis
   ```
## Data Sources
The project leverages patent data from:

- Google Patents
- WIPO
- USPTO
- FPO
- Espacenet
## Usage
- **Data Scraping:** Use Patents_Scraping.ipynb to collect and store patent data.
- **ETL Process:** Run the ETL_PROCESS.ipynb notebook to clean, transform, and prepare the data.
- **Visualization:** Load the processed data into Power BI or Python notebooks to generate insights.
  
## Contributions
Contributions are welcome! Follow these steps:

1. Fork this repository.
2. Create a new branch: git checkout -b feature/new-feature.
3. Commit your changes: git commit -m "Add new feature".
4. Push to the branch: git push origin feature/new-feature.
5. Submit a Pull Request.
   
## Contact
For questions, feedback, or collaborations, contact:

Najma Elboutaher
Email: najmaelboutaher@gmail.com

## Acknowledgments
Special thanks to all contributors and the open-source libraries used in this project.


