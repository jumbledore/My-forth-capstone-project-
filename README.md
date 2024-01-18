# My fourth capstone project

### Gender voice recognition by voice and speech analysis

![Screenshot of results]([https://github.com/jumbledore/My-fourth-capstone-project-/issues/1](https://github.com/jumbledore/My-fourth-capstone-project-/issues/1#issue-2085487086](https://private-user-images.githubusercontent.com/123168272/297281694-70a7bfc1-ce42-49a1-96ad-5bfd17f88dea.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MDU1NzA1MzIsIm5iZiI6MTcwNTU3MDIzMiwicGF0aCI6Ii8xMjMxNjgyNzIvMjk3MjgxNjk0LTcwYTdiZmMxLWNlNDItNDlhMS05NmFkLTViZmQxN2Y4OGRlYS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwMTE4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDExOFQwOTMwMzJaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT03MDk0ZWU1OTY5YjRjZjhlNjllZTJkNWQ0OGQ4NTZjNTk0M2JhZjYzMGZmZjYxZjQwMmRjZjIyZDQwYmQ2Y2FhJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.q6zj0XMjAeyFFd1kAOHb5slROkUpeJbLRJJg8vgNjS0))

#### Description of dataset

Dataset consists of 3,168 recorded voice samples, collected from male and female speakers. The voice samples are pre-processed by acoustic analysis in R using the seewave and tuneR packages, with an analyzed frequency range of 0hz-280hz (human vocal range).

#### General observations

- Both models have an F1 score of higher than 0.7; both models used will be good to help distinguish voice gender based on voice and speech data.
- CNN has a higher precision, recall and F1 score of 0.98; for the purpose of the data used, it is a better model.

### Addtional work done (convereting data into a picture and using CNN model for gender voice recognition)

#Original data
![Screenshot of original data](https://github.com/jumbledore/My-fourth-capstone-project-/issues/2)

The above data has 20 columns. To make it into a picture, we have to make the data into a (5*5) frame; add 5 more columns.

#Data with added 5 empty columns

![Screeenshot of original data with 5 additional empty columns](https://private-user-images.githubusercontent.com/123168272/297284469-283ac81a-410c-4c5b-9fc5-f384b8f2c336.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MDU0NzQyNDcsIm5iZiI6MTcwNTQ3Mzk0NywicGF0aCI6Ii8xMjMxNjgyNzIvMjk3Mjg0NDY5LTI4M2FjODFhLTQxMGMtNGM1Yi05ZmM1LWYzODRiOGYyYzMzNi5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwMTE3JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDExN1QwNjQ1NDdaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT05ZTU1YTEyMDE0NDYwNzFiMTg3MjYyNjZkNTFhZGRjMzgyMTJkYjA1ZWRjZWFiMTFhMWNkZWQ0MjFhNmYwMzFhJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.c145SOZAlB9Cjul-_2hLjjdW5nDdymQuYVuV-6tJS6A)


#Results

![Screenshot of data in image form](https://private-user-images.githubusercontent.com/123168272/297285205-3021247a-b664-414d-9541-56e89fe72300.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MDU0NzQ0NjAsIm5iZiI6MTcwNTQ3NDE2MCwicGF0aCI6Ii8xMjMxNjgyNzIvMjk3Mjg1MjA1LTMwMjEyNDdhLWI2NjQtNDE0ZC05NTQxLTU2ZTg5ZmU3MjMwMC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwMTE3JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDExN1QwNjQ5MjBaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1jY2RhZDA3MTNiYWIzNWUzZWE2ODA5NGIyZWFhMmRjZThhNjIyNTZjNTBhMmFiNTdiMzRjY2I1ZjVjZTQwNmNmJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.UBT1CBysUBn2-ZY79zVzt32hpQzbBqXf4fcMvE9uFtw)

# Heatmap and classification report using CNN model

![Heatmap and classification report based on CNN model](https://private-user-images.githubusercontent.com/123168272/297283144-088bf4bb-9e0a-45c2-b188-3a3f71dfdc21.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MDU0NzQ1NzgsIm5iZiI6MTcwNTQ3NDI3OCwicGF0aCI6Ii8xMjMxNjgyNzIvMjk3MjgzMTQ0LTA4OGJmNGJiLTllMGEtNDVjMi1iMTg4LTNhM2Y3MWRmZGMyMS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwMTE3JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDExN1QwNjUxMThaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT03MWMwODJkZWIzMTUwNWEzYWZmYTE0MDcwZDc4ZmVkYjNkM2MzMmMzYjVlYjVlZjA4MzA3OWEyMjY0YTgxNDZjJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.Dbh3VyiYw71yybMW0Ph5UHrCjnKvR-LlHOnkFPKPcwU)


#### Insights
- Data presented in a picture using CNN model (X) has a slightly lower F1 score compared to CNN model trained on raw data; this is due to additional inputs of empty data that has no correlation.
- X still has a high F1 score of 0.97 which meant that the model is also useful in helping to distinguish gender based on data presented in a picture.
- Based on the F1 scores of all 3 models, it strongly suggests that male and female voice can be distinguished based on the data provided.

[Link to LinkedIn](https://www.linkedin.com/in/jeremy-tay-116124139/)
