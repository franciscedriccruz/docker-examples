# Dockerfile, Image, Container 
# Dockerfile - blueprint for building images
# Image - template for running containers 
# Container - Packaged project

# Select base image from Dockerhub
FROM python:3.8 

# Add file to destination in container 
ADD main.py . 

# Install dependencies
RUN pip install requests beautifulsoup4 

# Specify entry command
CMD ["python", "./main.py"]

## To build image 
# docker build -t <name of image> <destination>
# docker build -t python-imdb .

## To run image
# docker run <image>
# docker run python-imdb

## To run image with proxy terminal with user input 
# -t sudo terminal
# -i interactive mode
# docker run -t -i python-imdb