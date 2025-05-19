# Use a lightweight Python base image
FROM python:3.11-slim

COPY ./src app
# Set working directory
WORKDIR /app

# Copy requirements and install
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy the application code
COPY app.py .

# Expose port 80
EXPOSE 80

# Run the app
CMD ["python", "app.py"]

