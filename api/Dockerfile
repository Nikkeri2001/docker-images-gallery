# Dockerfile for the API service

# Use the official Python image as a base
FROM python:3.9

# working directory
WORKDIR /app

EXPOSE 5050

# Copy the Pipfile and Pipfile.lock to the working directory
COPY Pipfile Pipfile.lock ./

RUN pip install pipenv
RUN pipenv requirements > requirements.txt
RUN pip install -r requirements.txt

# Copy the rest of the application code to the working directory
COPY . ./

CMD [ "python", "main.py" ]