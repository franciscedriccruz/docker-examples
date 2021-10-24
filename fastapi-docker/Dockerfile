FROM python:3.8

# define working directory (start in workdir)
WORKDIR /fastapi/app

# Copy requirements.txt in working directory 
COPY requirements.txt . 

# Install dependencies
RUN pip install -r requirements.txt 

# copy folders from local app folder into working directory app folder in container
COPY ./app ./app 

CMD ["python", "./app/main.py"]

## Build image 
# docker build -t <name of image> <directory>
# docker build -t python-fastapi .

## To run with port mapping 
# docker run -p 8000:8000 python-fastapi