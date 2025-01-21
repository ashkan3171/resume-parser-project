# **Resume Parser and Clustering Project**

## **Overview**
This project is an AI-powered resume parser designed to automate the analysis of resumes. It preprocesses resumes, groups them into clusters based on their content, and assigns a score to each resume based on its relevance to specific job domains. This tool leverages TF-IDF vectorization, K-means clustering, and scoring algorithms for efficient and accurate resume analysis.

---

## **Features**
- Preprocesses resumes to clean and standardize text.
- Groups resumes into distinct clusters based on content similarity using K-means clustering.
- Assigns scores (0–10) to resumes, ranking them based on relevance to their cluster's key themes.
- Provides visualizations, including:
  - Clustering distribution (PCA plot).
  - Word clouds for top skills in each cluster.
  - Histogram of resume scores.

---

## **Technologies Used**
- **Python**
- **Libraries**:
  - `pandas` – For data manipulation.
  - `nltk` – For text preprocessing.
  - `scikit-learn` – For TF-IDF vectorization and clustering.
  - `matplotlib` – For visualizations.
  - `wordcloud` – For generating word clouds.

---

## **Project Workflow**

### 1. **Preprocessing**
- Removed stopwords, punctuation, and other noise.
- Tokenized and lemmatized text for standardization.

### 2. **Feature Extraction**
- Used **TF-IDF Vectorization** to extract numerical features from the resumes.
- Represented each resume as a vector of word importance.

### 3. **Clustering**
- Applied **K-means clustering** to group resumes into 5 clusters.
- Visualized clusters in 2D space using PCA.

### 4. **Scoring**
- Scored resumes based on their alignment with cluster-specific top words.
- Normalized scores to a 0–10 range.

---

## **Cluster Analysis**
### **Cluster 0: Java Development**
- **Top Words:** `java`, `developer`, `jsp`, `spring`, `technology`
- **Theme:** Resumes focusing on Java development and related technologies.

### **Cluster 1: Web and Python Development**
- **Top Words:** `python`, `project`, `web`, `application`, `cs`
- **Theme:** Resumes with a focus on Python programming and web development.

### **Cluster 2: General/Creative/Regional**
- **Top Words:** `january`, `art`, `fitness`, `blockchain`, `civil`
- **Theme:** Mixed resumes with creative and regional references.

### **Cluster 3: Data Roles**
- **Top Words:** `data`, `hadoop`, `management`, `business`, `team`
- **Theme:** Resumes related to data analysis, engineering, and business management.

### **Cluster 4: HR and ETL**
- **Top Words:** `hr`, `etl`, `engineering`, `informatica`, `knowledge`
- **Theme:** Resumes with HR-related skills and ETL knowledge.

---


## **Usage**

### **Run the Project**
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/repo-name.git
   cd repo-name
