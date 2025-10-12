# Use Python 3.11 base image
FROM python:3.11

# Set working directory
WORKDIR /app

# Copy requirements and install dependencies
COPY req.txt .
RUN pip install --no-cache-dir -r req.txt

# Copy project files
COPY . .

# Expose Django port
EXPOSE 8000

# Run Django server
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
