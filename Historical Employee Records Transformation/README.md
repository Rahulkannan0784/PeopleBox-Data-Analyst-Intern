# Historical Employee Records Transformation

## Objective
Transform current employee data from a columnar format into a historical, row-based versioning format suitable for database storage.

## Dataset
The dataset is loaded into a Pandas DataFrame using the read_csv() function. The dataset file name is 'input.csv'. It contains columns such as Employee Code, Manager Employee Code, Date of Joining, Date of Exit, Compensation, Compensation 1, Compensation 1 date, Compensation 2, Compensation 2 date, Review 1, Review 1 date, Review 2, Review 2 date, Engagement 1, Engagement 1 date, Engagement 2, and Engagement 2 date.

## Transformation Process
1. Loaded the dataset into a Pandas DataFrame.
2. Calculated Last Compensation as the maximum value among Compensation, Compensation 1, and Compensation 2.
3. Calculated Last Pay Raise Date as the maximum date among Compensation 1 date and Compensation 2 date.
4. Calculated Variable Pay as 10% of Last Compensation.
5. Calculated Tenure in Org as the difference between Date of Exit and Date of Joining.
6. Calculated Performance Rating as the average of Review 1 and Review 2 scores.
7. Calculated Engagement Score as the average of Engagement 1 and Engagement 2 scores.

## Output
The transformed data is stored in a new CSV file named 'output.csv'. It includes columns such as Employee Code, Manager Employee Code, Last Compensation, Compensation, Last Pay Raise Date, Variable Pay, Tenure in Org, Performance Rating, Engagement Score, Date of Joining, and Date of Exit.

## Repository Structure
- **input.csv**: The original dataset file.
- **output.csv**: The transformed data file.
- **script.py**: Python script for data transformation.
- **README.md**: This file, providing an overview of the project and documentation. See attached documentation for more details.

## Google ColabYou can also run this transformation process in Google Colab. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1gA72qtUEPAVmo3OYq9Y0F5oG0mpid8pq?usp=sharing)

## Documentation
For detailed documentation, please refer to the attached documentation file.

## Contributors
- Rahulkannan
- [rahulkannan0784@gmail.com](mailto:rahulkannan0784@gmail.com)


