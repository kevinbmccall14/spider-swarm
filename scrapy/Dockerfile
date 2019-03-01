FROM python:3

# Set the working directory to app
WORKDIR /app

# Install python requirements from file
ADD requirements.txt /app/requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Copy local code into work directory
ADD . /app

# Run the crawler when the container launches.
CMD scrapy crawl basic_crawler
