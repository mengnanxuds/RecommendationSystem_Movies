# Movie Recommendation System

Welcome to the Movie Recommendation System project! This repository demonstrates the application of various machine learning algorithms to build a personalized movie recommendation engine. The project combines data analysis, algorithm development, and backend server deployment to deliver a comprehensive solution for movie recommendations.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Directory Structure](#directory-structure)
3. [Technologies and Libraries Used](#technologies-and-libraries-used)
4. [Installation and Setup](#installation-and-setup)
5. [Usage](#usage)
6. [Machine Learning Algorithms](#machine-learning-algorithms)
7. [Backend Structure](#backend-structure)
8. [Data](#data)
9. [Contributors](#contributors)

---

## Project Overview

This project is a comprehensive Movie Recommendation System developed to showcase various machine learning algorithms for recommendation tasks. The project is divided into two main components:

1. **Algorithm Implementation**: Jupyter Notebooks containing step-by-step implementations of various algorithms.
2. **Backend Server**: A backend server that can be used to deploy the recommendation system for real-world applications.

The recommendation system aims to provide users with personalized movie recommendations based on user preferences, ratings, and other factors.

---

## Directory Structure

```
MovieRecommendationSystem
│
├── Algorithm_JupyterNotebook
│   ├── 1_linear regression minimum least squares.ipynb
│   ├── 2_linear regression gradient descent.ipynb
│   ├── 3_linear regression Sklearn.ipynb
│   ├── 4_knn code implementation.ipynb
│   ├── 5_kmeans code implementation.ipynb
│   ├── 6_tfidf code implementation.ipynb
│   ├── 7_LFM gradient drop code implementation.ipynb
│   ├── data.csv
│   └── .ipynb_checkpoints
│
├── archive
│   └── fileProcessing.ipynb
│
├── Project_MovieRecommendSystem
│   ├── .idea
│   ├── businessServer
│   ├── recommender
│   └── spark-warehouse
│
├── .gitignore
├── MovieRecommendSystem.iml
└── pom.xml
```

### Key Components:

- **Algorithm_JupyterNotebook**: Contains Jupyter Notebooks with implementations of different machine learning algorithms used in the recommendation system. Each notebook demonstrates a specific algorithm, such as linear regression, KNN, K-means clustering, TF-IDF, and latent factor models.
  - **1_linear regression minimum least squares.ipynb**: Demonstrates linear regression using the least squares method.
  - **2_linear regression gradient descent.ipynb**: Shows linear regression with gradient descent.
  - **3_linear regression Sklearn.ipynb**: Implements linear regression using Scikit-learn.
  - **4_knn code implementation.ipynb**: Implements the K-Nearest Neighbors algorithm.
  - **5_kmeans code implementation.ipynb**: Demonstrates the K-Means clustering algorithm.
  - **6_tfidf code implementation.ipynb**: Uses TF-IDF for text-based recommendations.
  - **7_LFM gradient drop code implementation.ipynb**: Implements the Latent Factor Model with gradient descent.
  - **data.csv**: Dataset used for training and testing the recommendation system.

- **archive**: Contains older or auxiliary notebooks used for data processing or exploratory analysis.
  - **fileProcessing.ipynb**: A notebook for processing and preparing raw data.

- **Project_MovieRecommendSystem**: Contains backend server code for deploying the recommendation system.
  - **.idea**: IDE configuration files for IntelliJ IDEA.
  - **businessServer**: Contains the business logic and API endpoints for the recommendation system.
  - **recommender**: The core recommendation engine that processes user data and generates movie recommendations.
  - **spark-warehouse**: An optional component for large-scale data processing using Apache Spark.

- **.gitignore**: A standard `.gitignore` file to exclude unnecessary files and directories from version control.

- **MovieRecommendSystem.iml**: An IntelliJ IDEA project file that helps manage project settings in the IDE.

- **pom.xml**: A Maven configuration file used to manage project dependencies and build processes for the backend server.

---

## Technologies and Libraries Used

- **Python**
  - Jupyter Notebooks
  - Scikit-learn
  - Pandas
  - Numpy
- **Java** (for backend server)
- **Apache Spark** (optional, for large-scale data processing)
- **Maven** (build tool for backend server)

---

## Installation and Setup

### Prerequisites:

- Python 3.x
- Jupyter Notebook
- Java Development Kit (JDK)
- Apache Maven

### Steps to Run the Project:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/MovieRecommendationSystem.git
   ```
2. Navigate to the project directory:
   ```bash
   cd MovieRecommendationSystem
   ```
3. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the Jupyter Notebooks to explore the algorithms.
5. To run the backend server:
   ```bash
   cd Project_MovieRecommendSystem
   mvn clean install
   mvn spring-boot:run
   ```

---

## Usage

The recommendation system can be used in the following ways:

1. **Exploring Algorithms**: Use the Jupyter Notebooks to understand the various machine learning algorithms used in building a recommendation system.
2. **Deploying the Backend**: Use the backend server to deploy a live recommendation system that can be integrated with front-end applications.

---

## Machine Learning Algorithms

The project implements the following algorithms:

1. **Linear Regression (Least Squares & Gradient Descent)**
   - Implemented using both the least squares method and gradient descent.
2. **K-Nearest Neighbors (KNN)**
   - A simple, instance-based algorithm for recommendations.
3. **K-Means Clustering**
   - Used to group similar users or items.
4. **TF-IDF**
   - Used for content-based filtering.
5. **Latent Factor Model (LFM)**
   - A collaborative filtering method based on matrix factorization.

---

## Backend Structure

The backend server is structured as follows:

- **businessServer**: Contains the business logic for the recommendation system.
- **recommender**: Core recommendation engine.
- **spark-warehouse**: Used for large-scale data processing (optional).

### Key Files:

- **pom.xml**: Maven configuration file.
- **MovieRecommendSystem.iml**: IntelliJ IDEA project file.

---

## Data

The dataset used for this project is provided in the `data.csv` file. This file contains user-item interactions, such as movie ratings, user IDs, and movie IDs. The data is structured in a tabular format with the following key attributes:

- **User ID**: Unique identifier for each user.
- **Movie ID**: Unique identifier for each movie.
- **Rating**: The rating given by a user to a particular movie (e.g., on a scale of 1 to 5).
- **Timestamp**: The time when the rating was provided.

This dataset is essential for training and evaluating the recommendation models. It can be used to build both collaborative filtering and content-based filtering models. The source of the dataset is a publicly available movie dataset, ensuring compliance with data privacy and usage guidelines.

---

## Contributors

- **Mengnan**: Project creator and main contributor.

### How to Contribute
We welcome contributions to improve the Movie Recommendation System project! Please follow these guidelines:

1. **Fork the Repository**: Click the 'Fork' button on the top right corner of this repository to create your own copy.
2. **Clone Your Fork**: Use the following command to clone your fork locally:
   ```bash
   git clone https://github.com/your-username/MovieRecommendationSystem.git
   ```
3. **Create a Branch**: Create a new branch for your feature or bug fix:
   ```bash
   git checkout -b feature/your-feature-name
   ```
4. **Make Changes**: Implement your changes and commit them with descriptive messages.
5. **Push Your Changes**: Push your branch to your forked repository:
   ```bash
   git push origin feature/your-feature-name
   ```
6. **Create a Pull Request**: Go to the original repository and create a pull request, describing your changes in detail.

Feel free to fork the repository and contribute to the project by submitting a pull request!

