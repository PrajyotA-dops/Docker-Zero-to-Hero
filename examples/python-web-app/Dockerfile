FROM python:3.12

# Set up the working directory
WORKDIR /app

# Copy application code and dependencies
COPY requirements.txt /app
COPY devops /app/devops

# Install Python packages
RUN pip install -r requirements.txt

# Set up the application
WORKDIR /app/devops

# Run the application
ENTRYPOINT ["python3"]
CMD ["manage.py", "runserver", "0.0.0.0:8000"]



