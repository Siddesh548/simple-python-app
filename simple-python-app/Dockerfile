# Use a lightweight Python base image
FROM python:3.9-slim

# Set a working directory for the application
WORKDIR /app

# Copy the requirements.txt file (if you have one)
COPY requirements.txt .

# Install dependencies using pip
RUN pip install -r requirements.txt  # Install dependencies from requirements.txt

# Copy the application code
COPY . .

# Expose the port where the Flask app runs (default is 5000)
EXPOSE 5000

# Set the Flask app entry point 
CMD ["python", "app.py"]
