# COVID-19 Open Research Dataset Challenge (CORD-19)

This project presents a comprehensive exploratory data analysis (EDA), outlier analysis, missing value analysis, correlation analysis, and data visualization on the CORD-19 dataset, which contains scientific articles related to COVID-19. The goal is to uncover key trends, missing elements, and notable patterns within the dataset, providing researchers with a quick and insightful overview.

---

## 📂 Project Content

- **Dataset Upload and Examination**

- Load the dataset `metadata.csv`  
  [CORD-19 Dataset (metadata.csv)](https://www.kaggle.com/datasets/allen-institute-for-ai/CORD-19-research-challenge/data?select=metadata.csv)

- ## 1. Dataset Information
  The **CORD-19 dataset** is a comprehensive and openly accessible resource that systematically compiles scientific publications related to the COVID-19 pandemic for use by researchers. Published by the **Allen Institute for AI**, this dataset contains **over one million records**.The accompanying **metadata.csv** file includes key metadata for each academic article, such as the title, abstract, author information, and publication date. In this study, the dataset was loaded, its structure examined, and it was prepared for conducting fundamental analyses.

#### Columns in `metadata.csv`

- **cord_uid**: Unique identifier for each CORD-19 article (same article may appear in multiple sources)
- **sha**: SHA-1 hash values of the PDF files, separated by semicolons if multiple
- **source_x**: Sources where the article was obtained (e.g., ArXiv, Elsevier, PMC, WHO), separated by semicolons
- **title**: Title of the article
- **doi**: Digital Object Identifier (DOI) of the article
- **pmcid**: PubMed Central ID of the article (starts with PMC)
- **pubmed_id**: PubMed ID of the article (integer)
- **license**: License type (e.g., cc-by, gold-oa, etc.)
- **abstract**: Abstract text of the article
- **publish_time**: Date of publication (YYYY-MM-DD)
- **authors**: List of authors (Last name, First name; separated by semicolons)
- **journal**: Journal where the article was published (raw text, not normalized)
- **mag_id**: Microsoft Academic Graph ID (deprecated)
- **who_covidence_id**: WHO-assigned unique article ID (e.g., "#72306")
- **arxiv_id**: Identifier in arXiv
- **pdf_json_files**: File paths for JSON-converted versions of PDFs (semicolon-separated)
- **pmc_json_files**: File paths for JSON-parsed versions of PMC XML files (semicolon-separated)
- **url**: All URLs related to the article (semicolon-separated)
- **s2_id**: Semantic Scholar ID of the article (usable with API)

  ### **Explotary Data Analysis (EDA)**

  - df.head(), df.tail(), df.info(), df.describe(include='all').T, df.shape, print(df.nunique()), df.duplicated().any()
    -Statistical summaries of numerical and categorical variables
    -Column types, unique values, and data distributions

### **Missing Value Analysis**

- Calculate the number and percentage of missing values for each column
- Visualize the distribution of missing values (e.g., bar plot, matrix plot, heatmap)

- ### **Outlier Analysis**
- Detection of outliers in numerical columns using the IQR method
- Calculation of standard deviation and skewness values to determine the appropriate outlier handling strategy
- Identification of outliers in variables such as publication year (using IQR thresholds)
- Presentation of outliers with boxplots and statistical summaries

- ### **Correlation Matrix**

- ### **Data Visualization**
  - Bar plot for distribution of publication sources
  - Pie chart for distribution of publication licenses
  - Bar plot of the top publishing journals
  - Line plot for the number of publications by year
  - Histogram/Distribution plot for abstract length

---

## 🚀 How to Use

1. **Requirements**

   - Python 3.x
   - Required libraries:
     ```bash
     pip install pandas numpy matplotlib seaborn missingno
     ```

2. **Dataset**

   - Download and add the file [CORD-19 metadata.csv](https://www.kaggle.com/datasets/allen-institute-for-ai/CORD-19-research-challenge/data?select=metadata.csv) to the project folder.

3. **Running the Notebooks**

   - Open and run step by step either `main.ipynb` using **Jupyter Notebook** or **VS Code**.

---

## 📁 File Descriptions

- **main.ipynb**  
  Contains the main analysis steps, statistical summaries, and visualizations.

- **metadata.csv**  
  The CORD-19 dataset (must be downloaded separately as described above).

## 📌 Notes

- The dataset contains a significant amount of missing and outdated records; these issues were considered during the analysis.
- The notebooks include explanations to support learners in **data science** and **data analysis**.
- Contributions and feedback are welcome via pull requests.

---

## 🔗 References

- [CORD-19 Dataset - Kaggle](https://www.kaggle.com/datasets/allen-institute-for-ai/CORD-19-research-challenge)

---

**Prepared by:**  
Nilay Güler
