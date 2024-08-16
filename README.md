# Finetwork Data Processing Project!

## Table of Contents

1. [Introduction](#introduction)
2. [Project Goals](#project-goals)
3. [Methodology](#methodology)
4. [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
    - [Running the Project](#running-the-project)
5. [Usage](#usage)
    - [Data Collection](#data-collection)
    - [Data Processing](#data-processing)
    - [Generating Reports](#generating-reports)
6. [Tools and Libraries](#tools-and-libraries)
7. [Contributing](#contributing)
8. [License](#license)
9. [Contact Information](#contact-information)

## Introduction

Welcome to the Finetwork Data Processing Project! This initiative is designed to transform how Finetwork handles and analyzes its data, providing professional insights and streamlined reporting. In the long term, our goal is to develop a sophisticated, user-friendly web platform that presents agent data in a visually appealing and educational manner, facilitating precise and relevant business decisions.

Currently, Finetwork's reporting process relies heavily on manual, error-prone methods. This project aims to revolutionize that approach by implementing a semi-automated data processing workflow as the first step. Our immediate objective is to reduce the manual workload by 90%, ensuring that reports are generated accurately and efficiently. By leveraging advanced data analysis tools such as Pandas and Rainbow CSV, we will deliver a robust solution that not only enhances productivity but also minimizes the risk of errors.

The semi-automated process is only the beginning. In phase three, we will achieve full automation, further enhancing the efficiency and reliability of Finetwork's reporting. This project underscores Finetwork's commitment to innovation and operational excellence, setting the stage for a future where data-driven insights are just a few clicks away. Join us on this exciting journey to unlock the full potential of Finetwork's data!

## Project Goals

### Introduction to Agile Methodology

Our project will follow Agile methodology, emphasizing iterative development, regular reviews, and continuous feedback. This approach allows us to remain flexible and open to changes, ensuring the project's success.

### Iterations Overview

#### First Iteration (MVP - Minimum Viable Product)
The goal of the first iteration is to develop a semi-automated system for data processing. In this phase, the IT team will manually clean and prepare the data. This includes:

- Removing unnecessary data.
- Ensuring .xls files are cleaned of all formats and converted into .csv files that are easy to work with.
- The system will transform these files and output a .csv file, which will then be formatted into a rich Excel file with appropriate colors and formats. The automation in this phase will focus on transforming the files by merging them, combining the data through relevant transformations, and creating the final result files.

#### Second Iteration
The second iteration aims to generalize all the transformation and preparation steps, moving towards full automation. This phase will also reformat the .csv files for easy reading by the end customer.

#### Third Iteration
The third iteration will eliminate the need for Excel files, presenting the data on a web page in a friendly, professional manner. The web page will feature:

- Navigation options for easy access to specific agents and data.
- Plots and charts to visualize the data effectively.
- Security protocols to ensure data access is restricted to authorized personnel.
- Current Phase: First Iteration

### Story 1: General Jupyter Notebook
The primary objective is to create a skeleton ensuring that the code cells in Jupyter notebooks work as expected. This involves:

- Planning the data handling process.
- Visualizing the initial data acquisition by the Notebook.
- Identifying necessary transformations.
- Defining the final product requirements.
- This story will utilize sample files and perform one sample transformation of each required type. It is the most crucial and extensive story, as it will provide the foundation for all subsequent stories.

### Stories 2, 3, 4, and 5: Specific Projects

Each of these stories will focus on one of the four different projects we will work on. These steps will be more straightforward if we execute Story 1 thoroughly.

### Current Status

We are currently in the middle of Story 1 of the first phase, laying the groundwork for the entire project.

By adhering to this structured approach, we aim to achieve our goal of providing Finetwork with a professional, efficient, and automated data processing and reporting system.

## Methodology

Our project adheres to Agile methodology, a flexible and collaborative approach to project management that emphasizes iterative development, continuous feedback, and adaptability. This methodology ensures that we can respond swiftly to changes and deliver high-quality results.

### Iterative Development

We break down the project into small, manageable iterations, each aimed at producing a functional segment of the final product. Each iteration involves planning, development, testing, and review phases. This allows us to gradually build up the project's functionality and make adjustments as needed based on feedback.

### Regular Sprints and Reviews

The project is divided into regular sprints, typically lasting two weeks. At the end of each sprint, we conduct a review session where the Data Analyst team evaluates the progress and the current state of the deliverables. This ensures that we are consistently meeting the project's goals and allows us to make necessary adjustments promptly.

### Continuous Feedback and Improvement

Continuous feedback is integral to our process. We maintain constant communication with the Data Analyst team, who ensure the accuracy and relevance of the data we receive and the transformations required. Their feedback helps us refine our processes and improve the quality of the final product. After each sprint, feedback is incorporated into the planning of the next iteration, fostering a cycle of continuous improvement.

### Collaboration and Flexibility

Our small, closely-knit team fosters a highly collaborative environment. We work closely with the Data Analyst team to design and review each sprint, ensuring that the tasks are well-defined and aligned with the project goals. This close collaboration allows for high flexibility, enabling us to quickly adapt to any changes or new requirements that arise during the project.

### Current Context

Communication: We have ongoing communication with the Data Analyst team to ensure that the data we receive from the customer is accurate and the final product meets the requirements.

- Testing: While we do not have a dedicated QA team, the Data Analyst team tests our code to ensure that the final .csv files are correct and useful.
- Sprint Reviews: Each sprint is meticulously planned and reviewed by the Data Analyst team, minimizing the risk of the final customer rejecting the data.
- MVP: We aim to present a Minimum Viable Product (MVP) within a month, which will be reviewed by the final customer. This early feedback will help us make necessary adjustments before moving forward with subsequent iterations.
- By adhering to these Agile principles, we aim to deliver a high-quality, fully automated data processing system that meets the needs of Finetwork, providing valuable insights and enhancing operational efficiency.

## Getting Started

### Prerequisites

Before you begin, ensure you have the following software and tools installed:

- Python 3.x
- Jupyter Notebooks
- Pandas library
- Rainbow CSV extension
- openpyxl
- load_workbook

### Installation

Follow these steps to set up the project environment:

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/yourproject.git
2. Navigate to the project directory:
   ```sh
   cd yourproject
3. Install the required libraries:
   ```sh
   pip install -r requirements.txt

### Data Preparation Guide

Before starting, you will need to access and prepare the initial files. After running the Jupyter notebooks, there will be additional post-processing steps required to make the final file ready for agents to review.

#### Initial Files

The files you will need to start with are:

- `Metabase.xls`
- `Informe de métricas históricas.csv`

The final file to be generated is:

- `OBJETIVO_CALL_INB_AGOSTO_24`

#### Accessing Initial Files

**Metabase**

*Explain the process here once the information is available.*

**Informe de métricas históricas.csv**

1. Follow the link: [Link]
2. Use your Amazon credentials to log in.
3. You should be redirected to this page:
   
   ![Screenshot](path/to/your/image)

4. Ensure you are selecting the correct date range:
   - Click on the settings wheel.
   - Select "Intervalo y rango de tiempo".
   - Make sure "A diario" and "Mes hasta la fecha" are selected.

   ![Screenshot](path/to/your/image)

5. Apply the necessary filters:
   - Click on the settings wheel.
   - Select "Métricas".
   - Ensure only "Contactos administrados entrantes" and "Contactos transferidos fuera" are selected.

6. Once everything is set, click on "Acciones" and then "Descargar CSV".
7. Ensure the file is named `Informe de métricas históricas` before adding it to the GitHub project.

#### Preparing the Metabase.xls File

1. After downloading the file, filter the Metabase data. We are only interested in certain data, so we will create separate sheets for each filter:

   - **Active**: Apply this filter. ![Little Image](path/to/your/image)
   - **Canceled**: Apply this filter. ![Little Image](path/to/your/image)
   - Continue with additional filters as needed.

2. For each sheet, ensure there is data available for every date. If any dates are missing, create a column with the missing dates. Pay special attention to the "PTE de firma" sheet, where this happens more frequently.

   ![Screenshot](path/to/your/image)

3. It does not matter whether the sheet contains values or if it is a pivot table. If you encounter issues adding columns in a pivot table, simply copy and paste the data as values.

4. Add a final sheet to the end of the Metabase file named `AGENTES`. This sheet will contain a list of agents that the program will read.

   - Obtain this list from the `AGENTES_METABASE` file located in the shared folder:
     ![Screenshot](path/to/your/image)

After completing these steps, the file will be ready to use in the Jupyter notebooks.

#### Running the Notebooks

1. Run all cells in the following notebooks in the specified order:
   - `inbound_global.ipynb`
   - `inbound_diario.ipynb`
   - `pivot_table.ipynb`

2. Download the transformed file named `OBJETIVO_CALL_INB_AGOSTO_24`.

3. Share this file with the Reporting team and make a copy for the agents.

#### Final Adjustments Before Sharing with Agents

Before presenting the data to the agents, perform the following steps:

1. **Sort Agents:**
   - Sort agents in `RankingA`, with the best performers at the top.
   - Sort agents in `RankingB`, with the best performers at the top.
   - Sort agents in `RankingC`, with the best performers at the top.

2. **Manual Adjustments:**
   - Manually add any missing service data for agents who didn't use their own credentials.

3. **Final Touches:**
   - Hide the following sheets: *Blablabla*.
   - Protect all sheets to prevent any changes without a password.


### Running the Project

To start the Jupyter Notebook and run the scripts, follow these instructions:

1. Start Jupyter Notebook:
   ```sh
   jupyter notebook
2. Open and run the appropriate notebook files:

- In the Jupyter Notebook interface, navigate to the desired notebook file and open it.
- Run the cells in the notebook to execute the code.
- By following these steps, you will set up the environment and be ready to work with the project files. If you encounter any issues during installation or execution, please refer to the documentation or seek support from the project maintainers.

## Usage

### Data Collection

As mentioned before (see [Methodology](#methodology)), this current phase is semi-automatic. The data is obtained from diverse sources, such as reports from supervisors and automatic reports from various tools. This data is then manually transformed into a .csv file with no formatting, and all necessary transformations to facilitate processing are applied manually beforehand. 

Once all data is clean and ready, it is placed in a folder that will be accessed from Jupyter. In that folder, the data will have descriptive names that include the campaign and the current date.

### Data Processing

The process involves several steps to ensure that all available data is correctly processed:

- **Daily Reports:** Reports are generated daily, and the data from previous days can change. Therefore, a loop is created to find every available file, and the loop will end when no more files are found.

- **File Naming and Loop:** Files are placed in the designated folder with names that include the campaign and date. The loop retrieves and updates all files, ensuring that the most recent data is processed.

- **Transformations:** Once all files have been updated, the necessary transformations are applied to generate the final report. This ensures that a daily report is obtained, which updates itself each day, and culminates in a comprehensive monthly report that includes all data changes.

### Generating Reports

Once all data is processed, the result is an unformatted .csv file. This file is then manually transformed into a readable Excel file, complete with colors and formats that enhance legibility.

Instructions for generating and exporting reports:

1. **Run the Jupyter Notebook:**
   - Start the Jupyter Notebook and open the relevant notebook file.
   - Ensure all data files are placed in the appropriate folder with descriptive names.

2. **Execute the Cells:**
   - Run the cells in the notebook to process the data files. The notebook will handle the loop to find and update all files.

3. **Export the Final Report:**
   - Once the data is processed, export the final report as a .csv file.
   - Manually format the .csv file into an Excel file with the desired formatting and colors.

By following these steps, you will be able to generate a daily report that updates itself and culminates in a comprehensive monthly report, ensuring that all data is accurate and up-to-date.


## License

This project is proprietary software and is the sole property of Daniel Martín Monge. Unauthorized copying, distribution, or modification of this project, via any medium, is strictly prohibited without the explicit permission of the owner.

### Author

- **Daniel Martín Monge** - Sole author and owner of the project.

### Acknowledgments

- **Data Analyst Team** - Contributing to the data analysis and validation process.

For any inquiries regarding the use or distribution of this project, please contact Daniel Martín Monge directly.


## Contact Information
Provide contact information for the project maintainer(s):

Name
Email
GitHub profile
   
